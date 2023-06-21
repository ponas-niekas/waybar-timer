# waybar-timer

This is a custom waybar timer module.

### Screenshots

##### Innactive timer
![Innactive timer](https://github.com/ponas-niekas/waybar-timer/blob/main/img/preview1.png)
<br/>

##### Minute timer setup dialog
![Minute Dialog](https://github.com/ponas-niekas/waybar-timer/blob/main/img/preview2.png)
<br/>
##### Date-time timer setup dialog
![Date time Dialog](https://github.com/ponas-niekas/waybar-timer/blob/main/img/preview3.png)
<br/>
##### Active timer
![Active timer](https://github.com/ponas-niekas/waybar-timer/blob/main/img/preview4.png)

### Depends on

- bash
- zenity
- dateutils

### Configuration example:
```css
#custom-timer.active {
  background-color: #red;
}
```

```jsonc
"custom/timer": {
    "tooltip": true,
    "return-type": "json",
    "exec": "$HOME/.config/waybar/modules/waybar-timer check",
    "on-click": "$HOME/.config/waybar/modules/waybar-timer minute_dialog",
    "on-click-right": "$HOME/.config/waybar/modules/waybar-timer datetime_dialog",
    "on-click-middle": "$HOME/.config/waybar/modules/waybar-timer stop",
    "interval": 1
}
```
