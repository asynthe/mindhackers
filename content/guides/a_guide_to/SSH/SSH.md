# SSH
---

[[SSHFS]]
[[system/linux/dotfiles/PuTTY]]

making a ssh key to authenticate with github account
create your key
```
$ ssh-keygen -t ed25519 -C temp@example.com
```

-t -> encryption
-C -> email

start up the ssh agent
```
$ eval "$(ssh-agent -s)"
```

create the config file
```
$ nv ~/.ssh/config
```


inside of the file
> Host *
> 	AddKeysToAgent yes
> 	IdentityFile $HOME/.ssh/id_ed25519

>$ ssh-add ~/.ssh/id_ed25519

now go to the github ssh page, until it ask you for the key, copy and paste
>$ cat ~/.ssh/id_ed25519.pub

test if it works with
>$ ssh -T git@github.com
