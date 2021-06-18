# Article - Basic HTML

### Project Setup

Create a new project folder in your projects directory. For this project, you'll want to use Git/GitHub to store your files. Setup a repository for this project and then open the project folder in Visual Studio Code.

### Creating an Article about Jellyfish

We're going to be building a web page that is going to contain an article about some of the interesting jellyfish that live in the ocean. We'll learn about the common HTML elements along the way.

### Create index.html

Create your new HTML page in your project folder. Don't forget to change the &lt;title&gt; element. 

### Common HTML Elements

We are going to cover the most common HTML elements \(about ten\) when building our article. There are many more elements, but it is more productive to focus on the most common ones first, without getting overwhelmed with a huge list that you can't remember.

An important point to keep in mind with each of these elements is that browsers provide default styling for most of these elements, such as margins, text color, and font size. These defaults can be overridden by your own styles.

{% hint style="info" %}
If you need further help with understanding these HTML elements, the [MDN HTML Element Documentation](https://developer.mozilla.org/en-US/docs/Web/HTML/Element) is a great reference.
{% endhint %}

### Headings - &lt;h1&gt;, &lt;h2&gt;, &lt;h3&gt;, &lt;h4&gt;, &lt;h5&gt;, &lt;h6&gt;

The use of headings and sub-headings to organize the content of the document is likely familiar to you from their use in Word and Google documents. These HTML heading elements serve the same purpose on a web page.

There are six different elements, ranging from &lt;h1&gt; representing the most important, down to &lt;h6&gt;, representing the least important. In practice, the headings h1, h2, and h3 are heavily used, but it is often difficult to consistently follow a hierarchical pattern of importance throughout a site for these smaller heading.

{% hint style="info" %}
There should only be a single h1 element on a page.
{% endhint %}

#### Defaults for h1 - h6

```markup
    <h1>Heading 1</h1>
    <h2>Heading 2</h2>
    <h3>Heading 3</h3>
    <h4>Heading 4</h4>
    <h5>Heading 5</h5>
    <h6>Heading 6</h6>
```

![](../../.gitbook/assets/image%20%28149%29.png)

#### A Typical Use of h1 - h3

![](../../.gitbook/assets/image%20%2840%29.png)

### Adding the Article Headings

There are going to be three different jelly fish that we will cover in our article. The title of the article is the most important heading, so we'll use &lt;h1&gt; for that, followed by each section on a particular jellyfish using &lt;h3&gt;.

```markup
<h1>Jellies From the Deep</h1>
<h3>Pink Jelly</h3>
<h3>Orange Jelly</h3>
<h3>Yellow Jelly</h3>
```

![](../../.gitbook/assets/image%20%28116%29.png)

### Paragraphs - &lt;p&gt;

The paragraph element is meant to display some descriptive text or a paragraph. Consecutive paragraphs will have space between them, just like in a book.

### Add some descriptive paragraphs.

A technique front-end developers use when they need to add filler text is to use place-holder text supplied by sites like [https://loremipsum.io/](https://loremipsum.io/). Just copy the generated text and place in in the body of your paragraph element.

![](../../.gitbook/assets/image%20%28125%29.png)

```markup
 <h1>Jellies From the Deep</h1>
 <h3>Pink Jelly</h3>
 <p>Lorem ipsum dolor sit amet, consectetur adipiscing 
     elit, sed do eiusmod tempor incididunt ut 
     labore et dolore magna aliqua. Egestas tellus 
     rutrum tellus pellentesque eu tincidunt tortor aliquam. 
     Tellus rutrum tellus pellentesque eu tincidunt tortor 
     aliquam nulla facilisi. Libero justo laoreet sit amet cursus 
     sit.
 </p>
 <p>Vel quam elementum pulvinar etiam non quam lacus 
     suspendisse. Tincidunt dui ut ornare lectus sit amet
      est placerat in. Lectus nulla at volutpat diam ut 
      venenatis tellus. Sed elementum tempus egestas sed. 
      Lectus vestibulum mattis ullamcorper velit sed. 
      Placerat orci nulla pellentesque dignissim enim. 
      Cursus mattis molestie a iaculis at erat pellentesque.
 </p>
```

### Images - &lt;img&gt;

{% hint style="info" %}
The img element is a self-closing element. There is no content allowed between the opening and closing tags, so the correct syntax is &lt;img/&gt;
{% endhint %}

#### Images are inline elements

This means that they only take up as much horizontal space as their width and it can effect how the content following it behaves. Here are three examples of an images positioned before, at the beginning and in the middle of a paragraph element. We'll learn more about inline vs block elements, but for now it's just important to be aware that a block element, such as a paragraph, always starts on a new line, whereas text following an image will flow immediately to the right on the same line.

![](../../.gitbook/assets/image%20%2871%29.png)

#### img element attributes

The &lt;img element is our first element that demonstrates the use of attributes on the element.

&lt;img src="images/pink-jelly.jpg" alt="jellyfish"&gt; 

* **src** - the location of the image file
  * can be the relative location of an image file within the project directory
  * can also be an URL to a remote image file.
* **alt** - text used to support accessibility and search engines, or to display fallback text in case the image cannot be loaded.

#### Image Guidelines

* The best format for images are jpeg, gif, or png.
* Save the image in the correct size for which it will be displayed so that it doesn't waste a lot of time downloading. If you need to crop or shrink an image, sites like [www.pixlr.com](www.pixlr.com) are a good choice.
* Store images in a special folder, named images, within the project to keep things organized.

#### Finding Place-holder Images

The first step for our article is to find some jellyfish images to include.

Just like we used place-holder text for our paragraph content, we often need place-holder images to use for development purposes. The sites [unsplash.com](http://unsplash.com) and [pexels.com ](http://www.pexels.com) are great sites that have a wide assortment of free images to use in your pages. Go to the site and search for and download three jellyfish images to use in your article.

Set the value of the src attribute to the relative path of the image. The relative path is the location of the image file relative to the HTML page where it is being referenced. 

```markup
<h1>Jellies From the Deep</h1>
<h3>Pink Jelly</h3>
<p>Lorem ipsum dolor sit amet, consectetur adipiscing 
    elit, sed do eiusmod tempor incididunt ut 
    labore et dolore magna aliqua. Egestas tellus 
    rutrum tellus pellentesque eu tincidunt tortor aliquam. 
    Tellus rutrum tellus pellentesque eu tincidunt tortor 
    aliquam nulla facilisi. Libero justo laoreet sit amet cursus 
    sit.
</p>
<p>Vel quam elementum pulvinar etiam non quam lacus 
    suspendisse. Tincidunt dui ut ornare lectus sit amet
     est placerat in. Lectus nulla at volutpat diam ut 
     venenatis tellus. Sed elementum tempus egestas sed. 
     Lectus vestibulum mattis ullamcorper velit sed. 
     Placerat orci nulla pellentesque dignissim enim. 
     Cursus mattis molestie a iaculis at erat pellentesque.
 </p>
<img src="images/pink-jelly.jpg" alt="jellyfish"/>
```

![](../../.gitbook/assets/image%20%28134%29.png)

### Videos - &lt;video&gt;

The video element also has a src attribute, which is used to specify the location of the video. There are a couple of additional attributes that need to be set to control the video. These are a special kind of attribute, called boolean attributes.

#### Boolean Attributes

Boolean attributes are attributes that do not have a value. Their presence or absence indicates their value. If they are absent, the value is false. If the attribute is present, the value is true. 

The following is a list of the boolean attributes we are going to set on the video element.

**controls** - indicates whether the control panel is present on the video. this is the place where the user can interact with the video, such as starting and pausing. 

**autoplay** - indicates whether the video should start immediately when the page loads.

**muted** - indicates that the sound should be turned off.  this is require in some browsers for autoplay to work, as it can be problematic for videos with sound to autoplay unexpectedly.

**loop** - continually replay the video.

### Add a Video at the Top of the Article

You can find free videos on the site [pexels.com](http://pexels.com). Experiment with removing the boolean attributes to make sure you understand how each one works.

{% hint style="info" %}
Create a new folder in your project directory called videos, and store your videos there.
{% endhint %}

```markup
<h1>Jellies From the Deep</h1>
<div>
    <video controls autoplay muted loop src="videos/jellyfish.mp4"></video>
</div>
```

![](../../.gitbook/assets/image%20%2880%29.png)

### Anchors - &lt;a&gt;

Anchors, also called hyperlinks, or just links, are connections to other HTML pages. You can create links that navigate away from the current page, which is the technique you would typically use when you want to navigate to another page within your site. Or, you can create links that launch a new browser window and leave your current page alone. We are going to use the second technique to create some links from our narrative to external sites about jellyfish.

We need to use the href attribute on the anchor tag to specify the URL for the target web page. Just do a search for jellyfish and find a random page to link to for the purposes of this exercise.

{% hint style="info" %}
Set the attribute target="\_blank" to have the target web page launch in a new browser tab instead of replacing the contents of the current tab.
{% endhint %}

```markup
<p>Lorem ipsum dolor sit amet, consectetur adipiscing 
    elit, sed do eiusmod tempor incididunt ut 
    labore et dolore magna aliqua. Egestas tellus 
    rutrum tellus 
    <a target="_blank"
       href="https://www.wonderopolis.org/wonder/are-jellyfish-made-of-jelly">
        pellentesque
    </a> eu tincidunt tortor aliquam. 
    Tellus rutrum tellus pellentesque eu tincidunt tortor 
    aliquam nulla facilisi. Libero justo laoreet sit amet cursus 
    sit.
</p>
```

The anchor text is underlined and a different color, to indicate a link in the text. In future lessons we'll learn more about how to style anchors.

{% hint style="info" %}
Be sure to test your link to make sure when you click on it a new browser window is launched instead of navigating away from you current page.
{% endhint %}

![](../../.gitbook/assets/image%20%28105%29.png)

### **Add a Caption Under the Photos**

```markup
<p><i>Sally Smith</i></p>
```

For the caption, we're just going to style it in italic, just to distinguish it from normal paragraph text.

![](../../.gitbook/assets/image%20%2868%29.png)

### Lists - &lt;ul&gt;, &lt;ol&gt;, &lt;li&gt;

Lists will be familiar to you, as you've probably created them in Word or Google Docs. There are two options: ordered and unordered. Each type of list requires the use of the container element to specific what type of list, and the inner elements for each list item.

We're going to create an unordered list of links to the sections on each jellyfish within the article.  Before we do that we need to introduce the concept of internal links.

### Linking to Page Elements

Most of the time the  &lt;a&gt; element sets the href attribute to the url of an external page with in the website, or a page within another website \(usually launches a new tab for this type\). But it is also possible to set the href attribute to the id of another element in the same page and this will cause that element to scroll into view. This is particularly useful for very long articles where there is an index to sections at the top and clicking on a link in the index scrolls the page down to the appropriate section. For our article we are going to use this technique to link the MEET THE JELLIES list items to their associated sections further down in the article.

To use this technique, the target element must have an id attribute and the href on the anchor element must be set to that id with a '\#" in front. In this example the &lt;li&gt; element in the first code block references the &lt;h3&gt; element in the second.

```markup
<video controls autoplay muted src="videos/jellyfish.mp4"></video>
<p>Vel quam elementum pulvinar etiam non quam lacussuspendisse. 
    Tincidunt dui ut ornare lectus sit amet est placerat in. Lectus nulla at volutpat diam ut venenatis tellus. Sed 
    elementum tempus egestas sed. Lectus vestibulum mattis ullamcorper velit sed.Placerat orci nulla pellentesque dignissim enim.
</p>
<h2>MEET THE JELLIES</h2>
<ul>
    <li><a href="#pink-jelly">The Pink Jelly</a></li>
    <li><a href="#orange-jelly">The Orange Jelly</a></li>
    <li><a href="#yellow-jelly">The Yellow Jelly</a></li>
</ul>
```

```markup
 <h3 id="pink-jelly">Pink Jelly</h3>
```

The following screenshot shows what the web page should look like at this point. There should be a section at the top with the video followed by a section for each jellyfish \(I've just included the first jellyfish, as they each have the same structure\).

![](../../.gitbook/assets/image%20%2816%29.png)

![](../../.gitbook/assets/image%20%2863%29.png)

### Pushing Changes to GitHub and Netlify

Refer to the steps in the section. Use the Netlify URL for your assignment submission.

