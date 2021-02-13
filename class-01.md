# Class 1

* ## Shay Howe’s intro to RWD
The Internet took off quicker than anyone would have predicted, growing like crazy. Now, for the past few years, mobile growth has exploded onto the scene. The growth of mobile Internet usage is also far out pacing that of general Internet usage growth.

These days it is hard to find someone who doesn’t own a mobile device, or multiple, connected to the Internet. In the UK there are more mobile phones than people, and should trends continue mobile Internet usage will surpass that of desktop Internet usage within the year.

With the growth in mobile Internet usage comes the question of how to build websites suitable for all users. The industry response to this question has become responsive web design, also known as RWD.

* * Responsive Overview

Responsive web design is the practice of building a website suitable to work on every device and every screen size, no matter how large or small, mobile or desktop. Responsive web design is focused around providing an intuitive and gratifying experience for everyone. Desktop computer and cell phone users alike all benefit from responsive websites.

The responsive web design term itself was coined, and largely developed, by Ethan Marcotte. A lot of what is covered in this lesson was first talked about by Ethan online and in his book Responsive Web Design, which is worth a read.

* * Flexible Layouts

Responsive web design is broken down into three main components, including flexible layouts, media queries, and flexible media. The first part, flexible layouts, is the practice of building the layout of a website with a flexible grid, capable of dynamically resizing to any width. Flexible grids are built using relative length units, most commonly percentages or em units. These relative lengths are then used to declare common grid property values such as width, margin, or padding.


* ## All About Floats

* * What is “Float”?

Float is a CSS positioning property. To understand its purpose and origin, we can look to print design. In a print layout, images may be set into the page such that text wraps around them as needed. This is commonly and appropriately called “text wrap”. Here is an example of that.

In web design, page elements with the CSS float property applied to them are just like the images in the print layout where the text flows around them. Floated elements remain a part of the flow of the web page. This is distinctly different than page elements that use absolute positioning. Absolutely positioned page elements are removed from the flow of the webpage, like when the text box in the print layout was told to ignore the page wrap. Absolutely positioned page elements will not affect the position of other elements and other elements will not affect them, whether they touch each other or not.


* * What are floats used for?

Aside from the simple example of wrapping text around images, floats can be used to create entire web layouts.

Clear has four valid values as well. Both is most commonly used, which clears floats coming from either direction. Left and Right can be used to only clear the float from one direction respectively. None is the default, which is typically unnecessary unless removing a clear value from a cascade. Inherit would be the fifth, but is strangely not supported in Internet Explorer. Clearing only the left or right float, while less commonly seen in the wild, definitely has its uses.

* ## Don’t Overthink It Grids

The vast majority of websites out there use a grid. They may not explicitly have a grid system in place, but if they have a “main content area” floated to the left a “sidebar” floated to the right, it’s a simple grid.

If a more complex layout presents itself, people often reach for a grid framework. They assume grids are these super difficult things best left to super CSS nerds. That idea is perpetuated by the fact that a lot of the grid systems they reach for are very complicated.

A block level element is as wide as the parent it’s inside (width: auto;). We can think of it as 100% wide. The wrapper for a grid probably don’t have much to do with semantics, it’s just a generic wrapper, so a div is fine.

* * Gutters

The hardest part about grids is gutters. So far we’ve made our grid flexible by using percentages for widths. We could make the math all complicated and use percentages for gutters as well, but personally I don’t like percentage gutters anyway, I like fixed pixel size gutters. Plus, we’re trying to keep too much thinking out of this.

The first step toward this is using box-sizing: border-box;. I like using it on absolutely everything.



* ## CSS Floats Explained By Riding An Escalator

The Clear Property
There is one more wrinkle that we have not discussed yet: the clear property. “Clear” allows elements to specify where they should align in comparison to the floated elements.

In the first picture of the “Floats” section, the two escalator riders were courteously standing on each side of the escalator. This allows others to pass them and move freely as they wish.

Let’s say that instead of having one floated left element and one floated right element, we instead had 3 floated left elements and 1 on the right. The three floated left elements would stack up in a line on the left if we also give them the “clear: left” property. But if they horizontally aligned with the floated right element, it could make it very difficult or even impossible for the normal flow of elements to pass

“Clear: left” tells each person floating left that they should align themselves behind the first element that is floated left. Depending on the size of the bottom two people, it could be challenging for any normal elements to squeeze through and occupy the space on the top right. So even good escalator practices can still lead to blockages.

One of the most frequent uses of the clear property is “clear:both”. This allows you to reset the flow of elements, as opposed to continuing to maintain a right, left and normal flow. It’s kind of like that guy on the escalator who takes up the whole space because he brought his suitcase.
He has escaped the three-flow system and reset the rules. Bad for people that want to run up the escalator? Sure. But it’s good if you want to stop anyone from passing.

Notice how this is different from the one gentleman at the beginning who stood in the middle of the escalator, behind a line of people who were doing the same. That was a one-flow system. “Clear: both” acknowledges that there may be up to three flows, and blocks the passage of any element that follows.

* ## SMACSS Official Documentation
What is it?
SMACSS (pronounced “smacks”) is more style guide than rigid framework. There is no library within here for you to download or install. There is no git repository for you to clone. SMACSS is a way to examine your design process and as a way to fit those rigid frameworks into a flexible thought process. It is an attempt to document a consistent approach to site development when using CSS. And really, who isn’t building a site with CSS these days?!