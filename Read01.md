### Responsive web design

building a website suitable to work on every device and every screen size, no matter how large or small, mobile or desktop.
![](https://lh3.googleusercontent.com/proxy/JDJA2E4LV0UjVAzKIO0Mlfk33musUNISYWV4W5BbJF4Pt_S4cYVOoNE4QBKdckXJ2ZHY38MGU2TGpRQ410v6mw6flxySPkFkzt6PT6EbEjD03qxFwJaDtYywNL-YqOh9YwXdUXbd)

### Responsive vs. Adaptive vs. Mobile

_Responsive_ generally means to react quickly and positively to any change.

while _adaptive_ means to be easily
modified for a new purpose or situation, such as change _which is most popular_.

_Mobiles_ generally means to build a separate website commonly on a new domain solely for mobile users.

### Main components of Responsive web design

1.flexible layouts

2.media queries.

3.flexible media.

1.  _flexible layouts_ is the practice of building the layout of a website with a flexible grid, capable of dynamically resizing to any width.

    Flexible grids are built using relative length units, most commonly percentages or em units. These relative lengths are then used to declare common grid property values such as width, margin, or padding.

2.  Media Query
    is a CSS technique introduced in CSS3.

        It uses the @media rule to include a block of CSS properties only if a certain condition is true.

    ![](https://i.ibb.co/HzMkqxr/media.png)

3.  flexible media
    . As viewports begin to change size media doesn’t always follow suit. Images, videos, and other media types need to be scalable, changing their size as the size of the viewport

![](./img/px.png)

### float

The float CSS property places an element on the left or right side of its container, allowing text and inline elements to wrap around it.

### Values

• left\
The element must float on the left side of its containing block.

right\
The element must float on the right side of its containing block.\

• none:
The element must not float.

### Clearing Floats:

• The Empty Div Method :

using empty div. `<div style="clear: both;"><g/div>`

• Overflow Method:
relies on setting the overflow CSS property on a parent element.

• The Easy Clearing Method

uses a clever CSS pseudo selector (:after) to clear floats.
