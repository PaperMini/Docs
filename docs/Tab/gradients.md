# Gradients 

MiniTab has support for nice colorful animations in both header and footer, by using MiniMessage's [phase](https://docs.advntr.dev/minimessage/format#gradient)
feature. The phase is essentially automatically incremented every tick and the gradient is then re-rendered.

## Create A Gradient In The TabList

```json
[...]
{
  "raw": "<gradient:red:blue:<x>>Welcome to my server</gradient>"
  [...]
}
```

The first tag, `<gradient:color:color:phase>` creates a new gradient between the two colors. The third argument, the phase, 
has to be set to `<x>`. MiniTab will then replace this with the appropriate phase to create a smooth animation.