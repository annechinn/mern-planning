# Container Elements - div/span

In the 1990's, before the div and span tags were introduced, there were very limited ways to organize the layout of the content on the page. Early web developers used "hacks" to find ways to do it, such as using transparent images to force space between sections and tables.

Before HTML5 was introduced, the **div \(short for division\)** and **span** HTML elements were the primary way web developers defined chunks of content within their HTML to target sections of the page for layout and styling. 

These elements do not have any meaning on their own. If you added either of these elements to your HTML, but didn't add any content between the start and end tags, there would be no change in the HTML output.  They just act as generic containers for content and the class attribute is used for targeting CSS styles for the element.

### div

The div element is used to organize large sections of content, such as for the overall page layout as in the image below.

![](../.gitbook/assets/image%20%28113%29.png)

```markup
<body>
<div class="container">
    <div class="header">header</div>
    <div class="menu">menu</div>
    <div class="navigation">nav</div>
    <div class="mainbody">main content</div>
    <div class="footer">footer</div>
</div>
</body>
```

```css
.header {
    height: 80px;
    background-color: grey;
}
   
.menu {
    height: 80px;
    background-color: #F0F0F0;
    border: solid 1px black;
}
   
.navigation {
    width: 20%;
    height: 500px;
    background-color: #696A6C;
    float: left;
}
   
.mainbody {
    width: 80%;
    height: 500px;
    background-color: #D4D0D0;
    float: right;
}
   
.footer {
    height: 60px;
    background-color: grey;
    clear: both;
    border: solid 1px black;
}
```

The div element is used for more than these very large organizational units of a site. It is also used throughout the content to group blocks of content of all sizes for targeted styling.

For example, in the form below, each of the form fields has a div that contains the field name and value pair and that div is then styled to layout the pair horizontally.

![](../.gitbook/assets/image%20%28164%29.png)

```markup
 <div class="left">
    <div class="input-group">
      <label for="customer_name">Name</label>
      <input id="customer_name" />
    </div>
    <div class="input-group">
      <label for="phone_number">Phone</label>
      <input type="tel" id="phone_number" />
    </div>
    <div class="input-group">
      <label for="email_address">Email</label>
      <input type="email" id="email_address" />
    </div>
    <!-- removed for clarity -->
</div>
```

### span

The span element is also a generic container element, but unlike the div element, which is a block element, the span element is an inline element. The span element is also used to contain content for styling purposes, but is used to style small sections of inline text. 

In the image below I have changed the CSS of the site to set the border color to red for all div elements and the border color to green for all span elements.

![](../.gitbook/assets/image%20%2834%29.png)

