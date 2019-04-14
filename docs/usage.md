# Heck Animations -- Documentation
  [Back to Documentation](./readme.md)

## Installation & Usage

### Installing
To install and use, you can 
<!-- either install via npm,

```bash
$npm i heck-animations --save
```

or -->
download and include the `heck-animations.css` file into your project and link to it in your HTML document.

```html
<head>
  <link rel="stylesheet" href="heck-animations.css" />
</head>
```


## Using Heck Animations
One of the goals of the Heck Animations library is to be very easy to integrate. To use, just: 
1. Include Heck Animations in your HTML document's `<head>` using a `<link>`.
2. Apply animations to your HTML Elements using the corresponding CSS classes.

### How to Use
- `heck-animate`, to announce the element will be animated.
- Class corresponding to the animation you would like.
- Optional: 
    - Delay class. Default value: 0s. 
    - Duration class. Default value: 1s.
    - Timing Function class. Default value: ease-in-out.
    - Iteration class. Default value: 1.

See available classes in [Classes Documentation](./classes/readme.md)