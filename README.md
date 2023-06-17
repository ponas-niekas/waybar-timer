# waybar-timer

This is a custom waybar timer module.


### Screenshots

##### Innactive timer
![Innactive timer](https://github.com/ponas-niekas/waybar-timer/blob/main/img/preview1.png)
<br/>

##### Simple timer setup dialog
![Simple Dialog](https://github.com/ponas-niekas/waybar-timer/blob/main/img/preview2.png)
<br/>
##### Complex timer setup dialog
![Complex Dialog](https://github.com/ponas-niekas/waybar-timer/blob/main/img/preview3.png)
<br/>
##### Active timer
![Active timer](https://github.com/ponas-niekas/waybar-timer/blob/main/img/preview4.png)

### Depends on

- zenity
- dateutils
- coreutils

#### Configuration example:
```css
#custom-timer.active {
  background-color: #red;
}
```

```jsonc
"custom/timer": {
    "tooltip": true,
    "exec": "$HOME/.config/waybar/modules/waybar-timer check",
    "on-click": "$HOME/.config/waybar/modules/waybar-timer simple_dialog",
    "on-click-right": "$HOME/.config/waybar/modules/waybar-timer complex_dialog",
    "on-click-middle": "$HOME/.config/waybar/modules/waybar-timer stop",
    "interval": 1
}
```
