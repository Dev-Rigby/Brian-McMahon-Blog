---
template: blog-post
title: Giving Life to Web Pages with CSS Animations
slug: cssanimations
date: 2021-04-04 23:26
description: An article on css animations and transitions
---
CSS transformation moves or changes the appearance of an element. CSS transformation uses a collection of methods to move or change standard html elements into a two or three dimensional space. It helps in the rotation, scaling, skewing, translation and positioning of elements on a web page. CSS transform only applies to transformable elements such as `<div>`. The transformations take effect based on actions performed by the user. The following methods are provided by CSS transformation and its usage:

1. The translate() method moves an element from its current position according to the parameters given for the X-axis and the Y-axis.
2. The rotate() method rotates an element clockwise or counter-clockwise according to a given degree.
3. The scale() method increases or decreases the size of an element (according to the parameters given for the width and height).
4. The skewX() method skews an element along the X-axis by the given angle
5. .The skewY() method skews an element along the Y-axis by the given angle.
6. The skew() method skews an element along the X and Y-axis by the given angles.
7. The matrix() method combines all the 2D transform methods into one.

<figure>
<iframe height="265" style="width: 100%;" scrolling="no" title="zYNzoVQ" src="https://codepen.io/rigbysupreme/embed/zYNzoVQ?height=265&theme-id=light&default-tab=css,result" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/rigbysupreme/pen/zYNzoVQ'>zYNzoVQ</a> by Brian
  (<a href='https://codepen.io/rigbysupreme'>@rigbysupreme</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

<figcaption>Example Using CSS Transformations</figcaption>
</figure>

CSS transformation should be used to define the appearance of a website for different devices because it helps with the position of elements on smaller and larger screens. The color scheme for a website and the complete appearance of the website can be defined in a CSS. It allows the programmer to adjust the presentation of web pages to different types of devices like printers, phones and desktops. CSS transformation makes the coding and maintenance of web pages much easier because changes only need to be made to the CSS as opposed to every html page.

CSS animation lets elements gradually change from one style to another without using Javascript or any other client side programming language. CSS animations make it possible to animate transitions from one CSS style configuration to another. Animations consist of two components, a style describing the CSS animation and a set of keyframes that indicate the start and end states of the animation's style, as well as possible intermediate waypoints. There are no restrictions as to how many properties one can change. In order for the animation to work you have to bind the animation to an element. The following are the property of CSS animation and its usage. 


1. @keyframes -  This property specifies the animation code. The animation will gradually change from the current style to the new style at certain times. Keyframes hold what styles the element will have at certain times.
2. Animation-name - This property specifies the name of the @keyframes animation. This is the name given to the animation property that will be referenced by the element using the animation.
3. Animation-duration - This property defines how long an animation should take to complete one cycle.
4. Animation-delay - This property specifies a delay for the start of an animation.
5. Animation-iteration-count - This property  specifies the number of times an animation should be played
6. Animation-direction - This property specifies whether an animation should be played forwards, backwards or in alternate cycles.
7. Animation-timing-function - Specifies the speed curve of the animation.
8. Animation-fill-mode - Specifies a style for the element when the animation is not playing (before it starts, after it ends, or both)
9. Animation - A shorthand property for setting all the animation properties


CSS animations change the elements smoothly and gradually from one state to another. CSS animations are great for bringing a navigation menu in from the side, or showing a tooltip. Animating with CSS is the simplest way to get something moving on screen. Though the animations can be defined in your CSS, you may have to use JavaScript to fully control the states. CSS animations can start running on their own or they can be started by a user action. An CSS animation executes as soon as the animation property is applied. Adding animation to CSS can be faster than using Javascript as it uses the browser to do the processing.





Resources:



<https://www.w3schools.com/css/css3_animations.asp>

<https://www.w3schools.com/css/css3_2dtransforms.asp>

<https://www.adobepress.com/articles/article.asp?p=2266739&seqNum=6#:~:text=This%20gives%20you%20more%20control,intrinsic%20to%20the%20specific%20elements>