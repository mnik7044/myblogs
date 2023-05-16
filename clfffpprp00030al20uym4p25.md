---
title: "Flexbox In CSS"
datePublished: Sun Mar 19 2023 13:29:27 GMT+0000 (Coordinated Universal Time)
cuid: clfffpprp00030al20uym4p25
slug: flexbox-in-css
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1679071293542/978cde39-9fae-4605-9523-30a53efae263.png
tags: flexbox, css, web-development, webdev, wemakedevs

---

### Introduction

In this blog, we will explore the key concepts of flexbox including flex container, flex items, main axis, cross axis and how to use properties like flex-grow, flex-shrink, and flex-basis to create flexible layouts. We'll also look at some everyday use of flexbox, such as creating a navigation bar and centering elements.

Whether you're a newbie or an advanced developer, flexbox is a powerful tool that can help you create modern, responsive layouts. So let's dive in and explore the world of the flexbox.

### What is this Flexbox?

Flexbox is a CSS layout module that provides a more efficient way to layout, align and distribute content in any container. It is a powerful tool for creating responsive layouts and can help simplify any complicated web designs.

The word flexbox came from two words, flexbox=flexible+box. Flexbox is not anything but a one-dimensional layout method for laying out elements in rows and columns.

### Some key features of flexbox

Some key features of flexbox are:

1. **Direction control**: With flexbox, we can control the direction in which items are displayed either row-wise or column-wise.
    
2. **Alignment**: It allows us to align items vertically and horizontally within a container and also to adjust the spacing between items.
    
3. **Responsive design**: One of the most important use of flexbox is that it makes it easy to create responsive designs that can adapt to different screen sizes and devices.
    

### How to initialize flexbox in your container?

Let the container where we want to add flexbox has a class of container we just need to change the display property to flex to initialize the flexbox.

```css
.container{
display:flex;
}
```

### How are the items aligned?

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679221300343/2e58a548-3b36-4e98-8e9f-75aa893e70f3.png align="center")

By default, the items are aligned in the above-shown way. Its that we can change the alignment after learning the flex properties.

### Basic Terms

Before moving any further I would like to discuss the basic terms mentioned in the above image,

* **Main Axis**: It is the default axis along which the flex items are changed.
    
* **Cross Axis**: It is the perpendicular axis in this case it is column-wise.
    
* **Main Start & Main End**: The items are placed into the container starting from the main-start side and going toward the main-end side.
    
* **Cross Start & Cross End**: This is just the same thing as the main start and main end just for the cross-axis.
    
* **Main Size**: The main size of a flex item is defined by the main axis of the flexbox layout. If the main axis is set to be horizontal (row), the main size of a flex item would be its width. If the main axis is set to be vertical (column), the main size of a flex item would be its height. Here the main axis is the width.
    
* **Cross Size**: The cross size of a flex item is defined by the cross axis of the flexbox layout. If the main axis is set to be horizontal (row), the cross-size of a flex item would be its height. If the main axis is set to be vertical (column), the cross-size of a flex item would be its width. Here the main axis is the height.
    

### Flex Properties

1. **Flex-Direction**: flex-direction defines the main axis along which flex items are laid in a flex container.
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679224207173/05aca5dc-1277-47d6-bd10-809dd6fdf7f2.webp align="center")

The above image is for a clear understanding of the property flex-direction.

Some of the flex properties used for flex-direction are:

* `row(default)`: Flex items are laid out horizontally from left to right, with the first item at the start of the main axis and the last item at the end.
    
* `row-reverse`: Flex items are laid out horizontally from right to left, with the first item at the end of the main axis and the last item at the start.
    
* `column`: Flex items are laid out vertically from top to bottom, with the first item at the start of the main axis and the last item at the end.
    
* `column-reverse`: Flex items are laid out vertically from bottom to top, with the first item at the end of the main axis and the last item at the start.
    
    ```css
    .container{
    flex-direction:row/row-reverse/column/column-reverse;
    }
    ```
    

1. **Flex-Wrap**: It determines whether flex items should wrap or not if they exceed the width of the container. The different properties are:
    

* `nowrap(default)`: It means that the flex items will not wrap, and will instead overflow the container if the width is exceeded.
    
* `wrap`: This value allows the flex items to wrap ifinto different lines. This property is used to avoid overflow.
    
* `wrap-reverse`: This value is similar to `wrap`, but the order of the flex items are going to be reversed.
    
    ```css
    .container{
    flex-wrap: wrap/wrap-reverse;
    }
    ```
    

1. **Justify Content**: The justify-content property is a property that is used to align the flex items along the main axis of a flex container. The different properties are:
    

* `flex-start(default)`: It aligns the flex items at the start of the container along the main axis.
    
* `flex-end`: It aligns the flex items at the end of the container along the main axis.
    
* `center`: It aligns the flex items center within the container along the main axis.(**Prolly the most used property)**.
    
* `space-between`: It distributes the flex items along the main axis, with the first item at the start of the container and the last item at the end of the container.
    
* `space-around`: It distributes the flex items along the main axis, with equal space between each item.
    
* `space-evenly`: It evenly distributes the flex items along the main axis with equal space between each item and the start and end of the container.
    

```css
.container
{
justify-content: flex-end/center/space-between/space-evenly/space-around;
}
```

1. **Align Items**: The align-items property is used to align flex items along the cross-axis of a flex container.
    

* `stretch(default)`: It stretches the flex items to fill the container along the cross-axis.
    
* `flex-start`: It aligns the flex items at the start of the container along the cross-axis.
    
* `flex-end`: It aligns the flex items at the end of the container along the cross-axis.
    
* `center`: It centers the flex items within the container along the cross-axis.
    

```css
.container{
display: flex;
align-items: flex-start/flex-end/center;
}
```

Now we have talked about the properties of the container it's time for us to switch to some properties of the items of the flexbox.

### Item Properties

1. `flex-grow`: It specifies how much the flex item should grow relative to the other flex items when there is extra space along the main axis.
    
2. `flex-shrink`: It specifies how much the flex item should shrink relative to the other flex items when there is not enough space along the main axis.
    
3. `flex-basis`: It specifies the initial size of the flex item before any growing or shrinking occurs.
    
4. `order`: It specifies the order in which the flex item should appear within the container. By default flex items have an order of 0.
    
5. `align-self`: It specifies how the flex item should be aligned along the cross-axis. It has the same properties of align-items such as `flex-start` ,`flex-end` & `center` .
    

### Flexbox Games

There are many ways to learn a certain skill I came to know about one such way when I posted about me learning flexbox on Twitter there was this guy who commented about a game that might help you to level up your flexbox skills. Try it out might help you all.

1. [https://codingfantasy.com/games](https://codingfantasy.com/games)
    
2. [https://flexboxfroggy.com/](https://flexboxfroggy.com/)
    

### Conclusion

In this blog post we have covered the basics of flexbox, how to create a flex container, how to align flex items along the main and cross axes, and how to use flex item properties to control the size, order, and alignment of individual flex items.

With a little more practice and implementation you can be a pro in making responsive layouts.

### Let's Connect

If you enjoyed this post and would like to stay updated on my work, feel free to connect with me on social media

* LinkedIn: Click [here](https://www.linkedin.com/in/nikhil-mishra-8a6710244)
    
* Github: Click [here](https://github.com/mnik7044)
    
* Twitter: Click [here](https://twitter.com/nikktwts?t=WxH0im12f-NtbUJGeV2Xsw&s=09)
    

I'm always open to new connections and networking opportunities, so don't hesitate to reach out and say hello. Thank you for reading!