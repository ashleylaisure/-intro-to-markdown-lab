![iphone graphic](https://plus.unsplash.com/premium_photo-1721955487786-76802cbf0812?q=80&w=1332&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D)

# Intro to Media Queries
**Media queries** enable responsive design by applying specific CSS styles based on the media type. This allows you to adjust the appearance of a page according to characteristics like screen size or orientation.

>Utilizing `@media` we can wrap CSS rules that apply under specific conditions. 

 Take for example a situation where you want a hotpink background that changes to lightblue when viewed on a mobile device. 

 ***The orginial CSS:***
```css
body {
    background-color: hotpink;
 }
```

 A ***media expression*** or test must be established, but first we must determine what circumstances the screen should stop being hotpink.

### Common viewpoint sizes based on device include: 
 + Mobile: 320px - 480px
 + Tablet: 481px - 767px
 + Desktop: 768px - 1199px
 + Large desktop: 1200px+



 >Range features can be prefixed with *min* or *max* to express the *minimum condition* or *maximum condition* constraints. 

The minimum viewport width for the color hotpink is 480px. 

```css
 body {
    background-color: hotpink;
 }

 @media (min-width: 480px) 
 ```
When the media query determins that the width is less than 480px it will compute ***true*** and the contained CSS rules will be applied.
 
 ```css
 body {
    background-color: hotpink;
 }

 @media (min-width: 480px) {
    body {
        background-color: lightblue;
    }
 }
```
Resulting in the background changing colors at widths below 480px.


![iphone graphic 2](https://plus.unsplash.com/premium_photo-1721955487745-a2c3aea86d1c?q=80&w=1332&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D)

For more information about media queries check out the [MDN docs.](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_media_queries/Using_media_queries)



