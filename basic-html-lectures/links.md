# Anchor

**Absolute URLs** use the entire URL, including the protocol \(**http://**\), to link to a page. These are usually used to link to an external site.

```markup
<a href="http://www.google.com">Google</a>
```

 **Relative URLs** are used to link to a file **relative** to the file in which you are adding the link element. The value of the href property will consist of two parts: path to file + file name.

```markup
<!-- .. indicates one level up -->
<a href="../page1.html">Page 1</a>

<!-- same folder -->
<a href="page2.html">Page 2</a>

<!-- down into subDir folder -->
<a href="subDir/page3.html">Page 3</a>
```

| Title | Element | Attribute | Description | Self-closing |
| :--- | :--- | :--- | :--- | :--- |
| Link | a | href | A link within or between documents | False |
|  |  |  | The value of the href atrribute can be the url of another page within the site, or a remote site. Or it can be the id of an element within the current page.  |  |
|  |  | target | The value of "\_blank" opens the linked to page in a new window. |  |
|  |  | title | The browser may show this as a tooltip when the user hovers over the link. |  |

