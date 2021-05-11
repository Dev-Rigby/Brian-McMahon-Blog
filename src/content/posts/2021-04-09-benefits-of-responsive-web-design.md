---
template: blog-post
title: CSS Media Queries and Responsive Design
slug: responsive_css
date: 2021-04-09 13:30
description: An Article on CSS Media Queries and Responsive Practices.
featuredImage: /assets/nordwood-themes-ubiwo074qlu-unsplash-1-.jpg
---
When designing a website one must consider all of the different screens and interfaces that are going to try and access that website. As you probably know, a desktop site does not work well on mobile. This is where CSS responsive design comes in. Responsive design is when the design of a website is made to work on any device and screen. A good way to go about creating a Responsive design is working mobile first, the process of designing a website for mobile screens before other screens. This design process makes it easier ta adjust the design based on the users screen size. In this article I will go through two methods for creating a responsive web page, using CSS media queries and not using them.

Responsive Web design practice consists of flexible grids and layouts, images and use of CSS. Page elements are rearranged as the viewport grows or shrinks, and it relies on proportion-based grids to rearrange content and design elements.  It uses breakpoints to determine how the layout of a site will appear: one design is used above a breakpoint and another design is applied below that breakpoint. The breakpoints are commonly based on the width of the browser.

Responsive web design is a great way to adapt a full site to mobile devices without having to create a brand-new mobile site or mobile application. Because there is only one code base, the maintenance is easier and significantly less as the code does not have to change as new devices become available in the marketplace. When operational changes are needed, the change only has to be made once. Also, it is easier to gather analytical data as opposed to monitoring multiple websites. The website is more consistent because all data is centralized. The changes and rearrangements of the pages happen on the browser side. The page’s design and development respond to the user’s behavior based on the screen size, platform, and orientation. The adaptability and flexibility of these websites helps attract a wider audience and provide a good experience.

CSS media queries allow the developer the option to have different styles based on the users current screen size. Media queries work even better when they are used in a component-by-component basis. Seeing as not every part of the webpage is going to break at the same points, so breaking down the site into resizable components allows for a good flow. These breakpoints are where media queries shine. When a media query is included the website can be adjusted to fit any screen. The most common media query to use when creating a responsive design is, `@media screen and (min-width: X)`, where X is the screen width (usually in pixels). With in the following code block the developer can put styles that will only be used if the screen is at least the minimum screen width. This takes advantage of CSS’s cascade to override styles for the smaller screens. The most common execution of media queries is a one column mobile website that expands outward as the screen grows.

Below is example code of how one might use media queries to adjust elements on the screen as the screen grows.

```scss
@media screen and (min-width:560px) {
     .nav {
          &__toggle {
               display: none;
          }
          &__menu {
               flex-direction: row;
               li {
                    display: block;
                    margin-right: 3rem;
               }
          }
      }
}
```

CSS media queries are not the only method of building a responsive site. Responsive design can be accomplished through layout choices paired with grid or flex-box. Another method that instead defines how the styles scale rather than changing them completely for each size and is done by building your site to expand in columns. This can be referred to as “N columns to M columns to P columns to 1 column,” meaning that as the screen size decreases so do the number of columns of content. This is accomplished through a mathematical algorithm that uses the current screen size to calculate the number of columns permitted. The number of columns permitted is defined through the logic of wrap and clamp functions. I would recommend this method to advanced developers as it is more difficult and logically intense than CSS media queries.

Whether you prefer to use logic or CSS media queries, Responsive design is one of the most important facets of web design today. Handling how the end user engages with your content, gives control over the image that is presented. Webpages are often how companies and people represent themselves online. Responsive design allows those webpages to reach as many people as possible.

**Resources**

<https://dev.to/dailydevtips1/using-min-width-media-query-for-mobile-first-design-23op>

<https://dev.to/afif/build-your-responsive-website-without-media-query-omj>

<https://www.smashingmagazine.com/2011/01/guidelines-for-responsive-web-design/>

<https://www.nngroup.com/articles/responsive-web-design-definition/>