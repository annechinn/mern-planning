# Structure

### HTML is a Markup-Language

A mark-up language is different than a programming language. It doesn't have any programming logic or code that is executed to perform some action. It just allows you to annotate the text in the document to provide extra meaning to the content. The browser uses those annotations to know how to display the page. 

The mark-up language consists of two main concepts to understand:

**Elements** are the building blocks for defining the hierarchical structure of the page. An element consists of a starting tag and an end tag. In between the two tags is the content for that element. The content can, and often does, contain nested elements.

![](../.gitbook/assets/image%20%2827%29.png)

### Opening and  Closing Tags are Required

Unless the element is a self-closing tag, the element must have both a start and ending tag.

What's wrong with the HTML below?

```markup
<body>
    <h1>This is the title
        <p>Lorem ipsum dolor sit amet, consectetur 
        adipiscing elit, sed do eiusmod tempor incididunt 
        ut labore et dolore magna aliqua. 
        Ut enim ad minim veniam</p>
</body>
```

{% hint style="info" %}
**Self-closing tags** are an infrequent exception where the element is not allowed to contain any content between the opening and closing tag. In this case, there is a single starting tag  and it is closed with a forward slash, such as &lt;br/&gt;, which is used to indicate a line break. 

For a full list of the self-closing elements, see the [MDN Documentation](https://developer.mozilla.org/en-US/docs/Glossary/Empty_element).
{% endhint %}

### HTML Elements are Nested

Notice how the elements are in a nested structure. Proper nesting is required for the HTML to be valid.

```markup
<ol>
  <li>Item 1</li>
  <li>
    Item 2
    <ul>
      <li>Subitem 1</li>
      <li>Subitem 2</li>
    </ul>
  </li>
  <li>Item 3</li>
</ol>
```

What's wrong with the HTML below?

```markup
<body>
    <div>
        <p>This is a paragraph</div></p>
</body>
```

### Browsers are Forgiving

While there are ways to enforce HTML code to follow the rules, browsers have always attempted to gracefully handle errors in HTML. The HTML that currently exists is full of such errors, so it is not possible to change this behavior. 

It's up to you to carefully review your HTML to make sure the syntax is correct, otherwise you'll get unexpected results.

### White-space in HTML is ignored

You can add as much white-space as you want within the text of an element, and it will be ignored.

```markup
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, 
        sed do eiusmod tempor incididunt ut labore et dolore 
        magna aliqua. Ut enim ad minim veniam, quis nostrud 
        exercitation ullamco laboris nisi ut aliquip ex ea 
        
        a
        a
        as  b
        s fsd
         g sdfa g
        
        
        
        commodo consequat. Duis aute irure dolor in reprehenderit 
        in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
         Excepteur sint occaecat cupidatat non proident, 
         sunt in culpa qui officia deserunt mollit anim id est laborum.
    </p>
```

![](../.gitbook/assets/image%20%2820%29.png)

### Comments are Ignored

Anything that starts with **&lt;!-- and ends with --&gt;** will be completely ignored by the browser. ****This is useful for documenting your code and making notes to yourself, or for commenting out HTML that you are debugging.

```markup
<body>
    <!-- This will be ignored -->
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, 
        sed do eiusmod tempor</p>
    <!-- <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, 
        sed do eiusmod tempor</p> -->  
</body>
```

