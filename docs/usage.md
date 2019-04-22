# Heck Animations -- Documentation
  [Back to Index](./readme.md)

## Installation & Usage

### Installing
To install and use, you can include the `heck-animations.css` file into your project and link to it in your HTML document.

Download Heck-Animations into your project and link to it locally,

```html
<head>
  <link rel="stylesheet" href="heck-animations.css" />
</head>
```
or link to the latest version using GitCDN.

```html
<head>
  <link rel="stylesheet" href="https://gitcdn.link/repo/julian-hecker/heck-animations/master/dist/css/heck-animations.min.css" />
</head>
```
<!-- or install via npm

```bash
$npm i heck-animations --save
```
-->

## Using Heck Animations
One of the goals of the Heck Animations library is to be very easy to integrate. To use, just: 
1. Include Heck Animations in your HTML document's `<head>` using a `<link>`.
2. Apply animations to your HTML Elements using the corresponding CSS classes.

### How to Use
- `ha-animate`, to announce the element will be animated.
    - Default namespace of `ha-` can be changed in `src/scss/settings/_namespace.scss`
- Class corresponding to the animation you would like.
- Optional: 
    - Delay class. Default value: 0s. 
    - Duration class. Default value: 1s.
    - Timing Function class. Default value: ease-in-out.
    - Iteration class. Default value: 1.

See available classes in [Classes Documentation](./classes/readme.md)
