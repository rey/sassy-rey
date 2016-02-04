# sassy-rey

These are a collection of `sass` mixins and functions that I use on the regular.

## Mixins

### bootstrap-breakpoint

```
body
  // Default `background-color` is pink
  background-color: pink
  // from the `sm` breakpoint upwards turn orange!
  +breakpoint(sm)
    background-color: orange
```

### border-radius

```
.box
  // `.box` has a 5px radius!
  +border-radius(5px)
  border: 1px solid
  height: 100px
  width: 100px
```

### box-shadow

```
.box
  // Give the `.box` a box-shadow with `5px` horizontal offset, `10px` vertical
  // offset, `15px` blur, `20px` spread with a colour of red
  +box-shadow(5px, 10px, 15px, 20px, red)
```

### box-sizing

```
.box
  // I'm using `border-box` box sizing!
  +box-sizing(border-box)
  border: 1px solid
  height: 100px
  padding: 20px
  width: 100px
```

### background-gradient-top-to-bottom

```
.box
  // Wow such gradient!
  +background-gradient-top-to-bottom(pink, red)
  height: 100px
  width: 100px
```

### font-face

```
+font-face(font-name-light, #{$fonts_dir}font-name/light)
```


### font-smoothing

```
body
  // So smooth!
  +font-smoothing
```

### input-placeholder

```
input[type=text]
  // Turn the placeholder text `red`
  +input-placeholder
    color: red
```


### o

```
.box
  // Woo outline `.box` with a `red` er, outline!
  +o
```

### b

```
.box
  // Woo make the `background-color` of `.box` `red`
  +b
```

### text-shadow

```
h1
  // Give the `h1` a text-shadow with `5px` horiontal offset, `10px` vertical
  // offset, `15px` blur with a colour of `red`
  +text-shadow(5px, 10px, 15px, red)
```

## Functions

### opaque

```
.box
  // Make the background `red` with an opacity of 0.5! Cheers!
  background-color: opaque(red, 0.5)
```

### shade

```
.box
  // Woo give the `background-color` of `.box` a 10% shade
  background-color: shade(red, 10%)
```

### tint

```
.box
  // Woo give the `background-color` of `.box` a 10% tint
  background-color: tint(red, 10%)
```
