# Text-formatting Elements

| Purpose | Element | Description | Self-Closing |
| :--- | :--- | :--- | :--- |
| Headings | h1, h2, h3, h4, h5, h6 | Six levels of section headings | False |
| Paragraphs | p | Section of text, like in print | False |
| Line Break | br | Separates content with a carriage-return | True |
| Horizontal Rule | hr | A line to separate content | True |
| Lists | ul, ol, li | Ordered and unordered lists | False |
| Text emphasis | em | Emphasizes text | False |
| Text importance | strong | Singles out important text | False |
| Bold | b | Changes text to bold | False |
| Italic | i | Changes text to italic | False |
| Blockquote | blockquote | A quote, with optional citation | False |



### Emphasizing Text - &lt;strong&gt;, &lt;em&gt;, &lt;b&gt;, &lt;i&gt;

The use of these elements is often confusing, as it appears that their usage overlaps. This is a topic that is worth reviewing at a later point on the [MDN Documentation](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/strong#usage_notes).

| **Element** | **Usage** |
| :--- | :--- |
| strong | indicates that its contents have strong importance, seriousness, or urgency. Browsers typically render the contents in bold type |
| em | marks text that has stress emphasis |
| b | is used to draw the reader's attention to the element's contents, which are not otherwise granted special importance |
| i | represents a range of text that is set off from the normal text for some reason, such as idiomatic text, technical terms, taxonomical designations, among others |

{% hint style="info" %}
 The `<strong>` element is for content that is of greater importance, while the `<b>` element is used to draw attention to text without indicating that it's more important.

 While `<em>` is used to change the meaning of a sentence as spoken emphasis does \("I _love_ carrots" vs. "I love _carrots_"\), `<strong>` is used to give portions of a sentence added importance \(e.g., "**Warning!** This is **very dangerous.**"\) 
{% endhint %}

