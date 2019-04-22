# Heck Animations -- Documentation
  [Back to Index](../readme.md)

## Utility Classes

### Namespacing
All classes in the Heck Animations library are prefixed with a default namespace of `ha-`. 
Keep this in mind while browsing the documentation.

> This can be changed in the `_namespace.scss` file at `src/scss/settings/`.

### Animate Class
Use `ha-animate` on any element you would like to animate. This provides the optimal default settings for an animation.
You must also add an animation class for the animation to work. ([See Animation Classes](../animations/readme.md))

### Duration
You can use the classes "`ha-duration-`*duration*" or "`ha-dur-`*duration*" to set the duration of an animation. 
By Default, *duration* can either be a label, like `sm`, or the number of milliseconds, like `200`.

For example, you can use `ha-dur-1500` or `ha-duration-xxxl` to make an animation last 1.5 seconds.

The default available values for times (in milliseconds) and labels are as follows:

|   Durations   |
|---------------|
| xxxs  | 20    |
| xxs   | 50    |
| xs    | 100   |
| sm    | 200   |
| md    | 300   |
| lg    | 500   |
| xl    | 750   |
| xxl   | 1000  |
| xxxl  | 1500  |
| xxxxl | 2000  |

> This can be changed in the `_duration.scss` file at `src/scss/settings/`.

### Timing Functions
Use "`ha-timing-`*function*" or "`ha-`*function*" to set the timing function to be used by the animation. By default, this is set to `ease-in-out`.

> The full list of functions can be changed and viewed in the `_timing.scss` file at `src/scss/settings/`.

### Delay
You can use the classes "`ha-delay-`*delay*" or "`ha-del-`*delay*" to set the delay of an animation. 
By Default, *delay* can either be a label, like `sm`, or the number of milliseconds, like `200`.

For example, you can use `ha-del-1500` or `ha-delay-xxxl` to make an animation be delayed by 1.5 seconds.

The default values for times (in milliseconds) and labels are as follows:

|     Delays    |
|---------------|
| xxxs  | 20    |
| xxs   | 50    |
| xs    | 100   |
| sm    | 200   |
| md    | 300   |
| lg    | 500   |
| xl    | 750   |
| xxl   | 1000  |
| xxxl  | 1500  |
| xxxxl | 2000  |

> This can be changed in the `_delay.scss` file at `src/scss/settings/`.

### Iteration Count
Use "`ha-iteration-`*number*" or "`ha-`*number*", where *number* sets the number of times the animation will run. By default, *number* is a number from 1 to 10, or `infinite`. 

> This can be changed in the `_iteration.scss` file at `src/scss/settings/`.

Also by default, animations will alternate between backward and forward states.

### Direction
Use "`ha-direction-`*direction*" or "`ha-`*direction*", where *direction* is `in` or `out`. 
For example, setting the class `ha-out` will cause an animation to go from its end state to its starting state. `ha-fade` would cause the element to fade out, rather than in.

Animation Direction also affects the timing function that is applied to the element, essentially inverting it. This is automatically taken care of by the library.

### Play State
Use "`ha-running`" or "`ha-paused`" to let an animation run, or stop it from running. Default value: `running`.

## Conditional Animations
There are some conditions that will stop animations from running:
- Responsive
- Reduced Motion
- Print Media

### Responsive No-Animate
You can stop animations from running in specific viewport sizes by using the class `ha-no-animate-`*size*-*direction*, where *size* is `sm`, `md`, `lg`, `xl`, and where *direction* is `up` or `down`. 

For example, `ha-no-animate-md-down` will prevent animations from

> Viewport breakpoints are opinionated and can be changed in `_breakpoints_.scss` file at `src/scss/settings/`.

### Prefers Reduced Motion
If a user's device or browser settings prefer reduced motion, animations won't run.

In iOS, this can be changed by going into `Settings > General > Accessibility > Reduce Motion`.

### Print
Since paper can't be animated, animations won't run in print media.
