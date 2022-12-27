# Hugo
---
luke smith - internet independence
https://www.youtube.com/playlist?list=PL-p5XmQHB_JRRnoQyjOfioJdDmu87DIJc

luke smith
https://youtu.be/ZFL09qhKi5I
https://youtu.be/QTolhoxMyXg
https://youtu.be/jAXKSKb3etk
dt
https://youtu.be/927wgzzNMEA

arch ->
gentoo -> `www-apps/hugo`

__structure of your page folder__

`config.toml` -> site configuration (it can be another format like `.yml`)
`/content` -> location for site pages
`/archetypes` -> defaults for new pages
`/layouts` -> templates used to format pages from `content` directory
`/themes` -> themes
`/static` -> css, and all the files that are not markdown
`/public` -> exported page deploy location

__usage__
create a new site
```
$ hugo new site <name>
```

create a new site with `.yml` extension for main configuration file
```
$ hugo new site <name> -f yml
```

now, inside the directory. you can run the server.
```
$ hugo server --noHTTPCache
add an alias 
$ alias hss='hugo server --noHTTPCache
```

creating a post
```
$ hugo new first.md
```
creating a post inside a directory
```
$ hugo new posts/first.md
```












you need a theme or template, in this case we will use lukesmith's theme.
```
$ git clone https://github.com/lukesmithxyz/lugo themes/lugo
```
add this line to your `config.toml`, which will specify the theme that is going to be used.
```
$ echo "theme = 'lugo'" >> config.toml
$ cp themes/lugo/static/style.css static/
```

the two files you are going to be using the most are the `content` folder and `static/style.css` (site/themes/theme-name/static/style.css)

```

```


`content` -> folder for markdown files
`static` -> folder for images, documents and anything else




__RUNNING__
generate the site, and put it in the `public` dir
```
$ hugo
```


```
$ hugo server
```





hugo new site -> create a new website
hugo new about.md -> create a new markdown file (in content)



if creating a file on /layouts that is the same name as the themes file, it will overwrite it in the webpage

there are two different types: _singles_ and _list_
<u>singles</u> = they have stuff and content, most of them go in the `/content` folder
<u>list</u> = Homepage is by default a list, and tags page too
