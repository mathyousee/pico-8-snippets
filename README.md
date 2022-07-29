# pico-8-snippets
Snippets for use with PICO-8 fantasy console game dev

## Aimed shot for shoot-em-up

Formula to determine the angle of the shot between the source(x1, y1) and target(x2,y2)

```lua
ang=atan2(y2-y1,x2-x1)
```

## Center text horizontally on a point

Function to print text centered on a specific X coordinate. In PICO-8 each character is 4 pixels wide by 6 pixels high(including gaps/spacing). This function wraps the standard print() function and offsets the `x` coordinate by half the total number of pixels in the text string: `#txt*4*0.5` becomes `#txt*2`. For the `y` coordinate, as this is a single line of text it is offset by a constant of `3` pixels.

```lua
function printc(txt,x,y,c) 
 print(txt,x-#txt*2,y-3,c)
end
```