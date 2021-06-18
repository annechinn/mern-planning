# Element Flow - Block/Inline

### Element Flow: Inline vs Block 

Every element on a web page is a rectangular box.  By default, elements flow from top to bottom, but the CSS display property is used to determine how much horizontal and vertical space an element takes up.

* **Block elements**: take up the entire line, unless they are empty.
* **Inline elements**: take up width of their content only.
* **Inline block elements**: like inline, except can specify width and height.

headings, paragraphs, lists are examples of block elements. images, links, spans are examples of inline elements.

![](../.gitbook/assets/image%20%28142%29.png)



### Every HTML Element is a Rectangular Box

Every element on a web page is a rectangular box. The **display property** in CSS determines just how that rectangular box behaves.

The default value for all elements is inline. Most “User Agent Stylesheets” \(the default styles the browser applies to all sites\) reset many elements to “block”. 

### display: inline

Elements only occupy the horizontal and vertical space occupied by its own content. The element sits "inline" with the rest of the text.

Examples include: span, b, img, a \([full list](https://developer.mozilla.org/en-US/docs/Web/HTML/Inline_elements)\)

![](../.gitbook/assets/image%20%28128%29.png)

An inline element will accept margin and padding, but the element still sits inline as you might expect. Margin and padding will only push other elements horizontally away, not vertically.

![](../.gitbook/assets/image%20%28144%29.png)

### display: inline-block

An element set to inline-block is very similar to inline in that it will set inline with the natural flow of text. The difference is that you are able to set a width and height which will be respected.

![](../.gitbook/assets/image%20%2870%29.png)

### display: block

A number of elements are set to block by the browser UA stylesheet. They are usually container elements, like paragraphs, lists, div, or some block elements, like headings. Block level elements do not sit inline. By default \(without setting a width\) they take up as much horizontal space as they can.  By default their height equals 0. It will fill vertically around content.

Examples: p, ul, li, h1, div \([full list](https://developer.mozilla.org/en-US/docs/Web/HTML/Block-level_elements)\)

![](../.gitbook/assets/image%20%28107%29.png)

### display: none

Hides the element from view. The element is still there, but not visible to the user.

![](../.gitbook/assets/image%20%2898%29.png)

### CodePen Samples

{% embed url="https://codepen.io/annechinn/pen/xxgjjZj" caption="span" %}

{% embed url="https://codepen.io/annechinn/pen/dyNeerx" caption="image" %}

{% embed url="https://codepen.io/annechinn/pen/MWJGXoz" caption="paragraph" %}

### Rules

* Inline elements cannot contain block elements
* Except for an anchor

```markup
<a href="section2.html">
   <h2>Section 2</h2>
   <p>All about food</p>
</a>
```

