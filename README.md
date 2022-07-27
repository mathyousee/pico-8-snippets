# pico-8-snippets
Snippets for use with PICO-8 fantasy console game dev

## Aimed shot for shoot-em-up

Formula to determine the angle of the shot between the source(x1, y1) and target(x2,y2)

```lua
ang=atan2(y2-y1,x2-x1)
```
