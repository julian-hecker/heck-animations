# Heck Animations -- Documentation
  [Back to Index](../readme.md)

## Utility Classes

### Namespacing
All classes in the Heck Animations library are prefixed with a default namespace of `ha-`. 
Keep this in mind while browsing the documentation.

> This can be changed in the `_variable.scss` file at `src/scss/settings/` in the Namespace section.

### Animate Class
Use `ha-animate` on any element you would like to animate. This provides the optimal default settings for an animation.
You must also add an animation class for the animation to work. ([See Animation Classes](../animations/readme.md))

### Duration
You can use "`ha-duration-`*ms*" or "`ha-dur-`*ms*" to set the duration of an animation, where *ms* is the number of milliseconds, from 100 to 2000 with increments in 100. This allows you to make an animation that is up to 2 seconds long. 

For example, you can use `ha-dur-1500` to make an animation last 1.5 seconds.

> This can be changed in the `_utilities.scss` file at `src/scss/utilities/` in the Duration section.

### Timing Functions
Use "`ha-timing-`*function*" or "`ha-`*function*" to set the timing function to be used by the animation. By default, this is set to `ease-in-out`.

> The full list of functions can be changed and viewed in the `_variable.scss` file at `src/scss/settings/` in the Timings section.

### Delay
Use "`ha-delay-`*ms*" or "`ha-del-`*ms*" to set the delay of an animation, where *ms* is the number of milliseconds, from 0 to 2000 with increments in 100. This allows you to make an animation that is delayed by up to 2 seconds long. 

> This can be changed in the `_utilities.scss` file at `src/scss/utilities/` in the Delay section.

### Iteration Count
Use "`ha-iteration-`*number*" or "`ha-`*number*", where *number* sets the number of times the animation will run. By default, *number* is a number from 1 to 10, or `infinite`. 

> This can be changed in the `_utilities.scss` file at `src/scss/utilities/` in the Iteration section.

Also by default, animations will alternate between backward and forward states.

### Direction
Use "`ha-direction-`*direction*" or "`ha-`*direction*", where *direction* is `in` or `out`. 
For example, setting the class `ha-out` will cause an animation to go from its end state to its starting state. `ha-fade` would cause the element to fade out, rather than in.

### Play State
Use "`ha-running`" or "`ha-paused`" to let an animation run, or stop it from running. Default value: `running`.

## Conditional Animations
There are some conditions that will stop animations from running:
- Responsive Classes
- Browser Support
- Reduced Motion
- Print Media

### Responsive Disabling
You can stop animations from working in specific viewport sizes by adding a class: `ha-off`*size*-*direction*, 

where *size* is `xs`, `sm`, `md`, `lg`, or `xl`, and

where *direction* is `up` or `down`. 

For example, the class `ha-off-md-up` will disable animations in medium viewports and above.

> Viewport breakpoints are opinionated and can be changed in `_variable.scss` file at `src/scss/settings/` in the Breakpoints section.

### Browser Support
Animations use `@supports` to test the browsers' support of the `animation-fill-mode: both` property to determine if animations should be displayed, as animations without supporting this property may break.

### Prefers Reduced Motion
If a user's device or browser settings prefer reduced motion, animations won't run.
In iOS, this can be changed by going into `Settings > General > Accessibility > Reduce Motion`.

### Print
Since paper can't be animated, animations won't run in print media.
