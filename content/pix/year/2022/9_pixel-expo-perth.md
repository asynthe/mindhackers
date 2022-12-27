DATE:
LOCATION:

![apple]({{ $image := resouces.Get "/img/apple.jpg" }})

{{ $image := resources.Get "/apple.jpg" }}

![]({{ $image := resources.Get "apple.jpg" }})
