# Prerequisites

- At least Java 23
- A [Paper](https://papermc.io) Server  

??? info "Spigot Fork Compatibility"
    Tab only works with [Paper](https://papermc.io) and derivatives, Spigot and Bukkit won't work!
    Spigot and Bukkit are "legacy" versions, that should not be used if not absolutely necessary!

# Installation

- Just drop the [jar](https://github.com/PaperMini/Tab/releases) into your plugin folder and restart the Server.

# Configuration

MiniTab is configured through the `plugins/Mini/Tab/config.json` file.

!!! note 
    When editing the config while running the server, make sure to always run `/mini:tab reload` after saving to apply the changes

## Example

```json
{
  "version": 1,
  "header": {
    "raw": "<gradient:red:blue:<x>>Hello, %player_name%!</gradient>",
    "animated": true,
    "animationSpeed": 0.1
  },
  "footer": {
    "raw": "<blue><b>Its an nice Day!</b></blue>",
    "animated": false,
    "animationSpeed": 0.0
  }
}
```

`header` -> Shown above the players  
`footer` -> Shown below the players  
`raw` -> MiniMessage String to display. Can use PlaceholderAPI  
`animated` -> If set to true, gradients will animate in the part of the Tablist  
`animationSpeed` -> the higher, the faster the animation  

??? important "Animation prerequisites"
    Animations are created by (ab)using the phase feature of MiniMessage. If you want to use them, have a look at [the gradient guide](tab/gradient.md)