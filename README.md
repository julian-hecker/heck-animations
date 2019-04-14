# Heck Animaitons
CSS Animation library for quickly bringing your pages to life!

Taking inspiration from [Daniel Eden's Animate.css](https://github.com/daneden/animate.css) and [Zurb's Motion UI](https://github.com/zurb/motion-ui) libraries.


## Installation & Usage
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

## Features
- Lots of pre-coded animations
- Customizable Namespacing
    - Prevents conflicts with other CSS.
- Support for *Reduced Motion*
    - Disables animations if user settings request it.
- Responsive Animations
    - Choose what viewport sizes your animations will display on!
<!-- COMING SOON

- Animate on Javascript event
- Synchronous animations
-->
## How to use
1. Include Heck Animations in your HTML document's `<head>` using a `<link>`.
2. Apply the following classes to the HTML Elements you wish to animate:
    - `heck-animate`, to announce the element will be animated.
    - Class corresponding to the animation you would like.
    - Optional: 
        - Delay class. Default value: 0s. 
        - Duration class. Default value: 1s.
        - Timing Function class. Default value: ease-in-out.
        - Iteration class. Default value: 1.
        
[See all class documentation](./docs/classes/readme.md) <!-- Create docs/classes.md/ -->

## Accessibility
Supports `prefers-reduced-motion` media query for motion-sensitive users; will disable moving animations, but allows opacity to still be animated.

## Compatability
Normally, browsers that do not support animations will cause animated components to break. By using the `@supports` query, Heck Animations prevents pages from being broken on older browsers. If animations (or @supports) are not supported, then elements will display normally and not animate.

## License
Heck Animations is licensed under the [MIT license](http://opensource.org/licenses/MIT).
