# Evolution of the Web Page

### Plain HTML

In the beginning, HTML \(Hyper Text Markup Language\) was just a way to send text documents  around the internet with links \(hyper text\) between documents. 

* 1995 - HTML1.2   -  Plain HTML - Text, Links, Images. No tables, to styling, no interactivity.
* 1999 - HTML 4.01 - Tables, CSS, JavaScript - Beginning of styling, interactivity
* 2016 - HTML 5 - Audio, Video, Canvas ****- Advances in styling, interactivity

![](../.gitbook/assets/image%20%2829%29.png)

### HTML/CSS/JAVASCRIPT

Modern web pages depend on two additional technologies beyond HTML: CSS and JavaScript. These three components provide the underpinning of every web page. 

All the front-end libraries and frameworks are just making it easier to create a web page that contain these three components.

So, let's breakdown these three components and what their individual purposes are. 

| Technology | Description |
| :--- | :--- |
| **HTML** | Hypertext Markup LanguageA _mark-up language_ to describe the content of web pages |
| **CSS** | Cascading Style Sheet - A _stylesheet language_ used to express the presentation of web pages. |
| **JavaScript** | A _programming language_ used for both front-end and back-end development. |

![](../.gitbook/assets/image%20%2859%29.png)

### Best Explained with Examples

### HTML/CSS - Resume

A good analogy for the HTML/CSS relationship within a web page is when you are creating a resume. 

<table>
  <thead>
    <tr>
      <th style="text-align:left"><b>HTML </b>- Text Content</th>
      <th style="text-align:left"><b>HTML </b>- Structure</th>
      <th style="text-align:left"><b>CSS - Style</b>
      </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">
        <p></p>
        <ul>
          <li>Personal Info</li>
          <li>Work Experience</li>
          <li>Education</li>
          <li>Extra-curriculars</li>
        </ul>
      </td>
      <td style="text-align:left">
        <p></p>
        <ul>
          <li>Headings</li>
          <li>Bullet List, Ordered List</li>
          <li>Paragraphs</li>
          <li>Image</li>
        </ul>
      </td>
      <td style="text-align:left">
        <p></p>
        <ul>
          <li>Colors</li>
          <li>Fonts</li>
          <li>Font-size</li>
          <li>Positioning</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

{% embed url="https://codepen.io/annechinn/full/LYxmMZJ" %}

### HTML/CSS - CSSZenGarden.com

The site [csszengarden.com](http://csszengarden.com) is a site that educates on the role CSS plays in design and has a link to provide both the HTML and CSS files separately and to view the impact CSS can make.

Go to the site, and click on the HTML FILE link to download the HTML file and then display that file in your browser by dragging in from your file explorer to a web browser window.

![](../.gitbook/assets/image%20%28131%29.png)

Below is the HTML with no CSS applied. Very basic, just text, links, and some standard headings.

![](../.gitbook/assets/image%20%2813%29.png)

### What a Difference CSS can Make!

Next, click on the VIEW ALL DESIGNS link and browse through each of the different design links on the right. Each of these designs has the exact same underlying HTML content, just a different stylesheet!

![](../.gitbook/assets/image%20%2852%29.png)

![](../.gitbook/assets/image%20%28119%29.png)

![](../.gitbook/assets/image%20%28132%29.png)

### CSS - Animation

{% embed url="https://codepen.io/everylastpixel/pen/QWybxmV" %}



### JavaScript - Animation

First, JavaScript can be used to add what I'd call eye-candy to the site. The content is all there, but it's dull without some action. JavaScript can be used to display the content in visually appealing ways and add movement with advanced animations. Below is an example of JavaScript being use in this capacity.

{% embed url="https://www.charles-richard.net/" %}

{% embed url="https://www.legworkstudio.com" %}

{% embed url="http://knowlupus.org" %}

{% embed url="https://www.sbs.com.au/theboat/" %}

{% embed url="https://mrdoob.com/projects/chromeexperiments/ball-pool/" %}



### JavaScript - Seamlessly Updates Content

* Users want a Desktop feel. No full page refreshes on changes.
* JavaScript communicates with back-end services to retrieve/update data.

\*\*\*\*

**Google Search Input** - A really good example of this is the Google Search screen. As the user types into the search input box, JavaScript is being used to communicate with the server and seamlessly retrieve and present relevant search strings based on what the user is typing.

{% hint style="info" %}
Take a look at the Console Developer Tools Network Tab to see the network traffic.
{% endhint %}

![](../.gitbook/assets/image%20%2817%29.png)



 **NY Times** - **Article Comments**

{% embed url="https://www.nytimes.com/2021/04/06/dining/croissant-recipes.html" %}

* Navigate to the article, click on the Comments button at the bottom
* JavaScript responds to the button click, sends as request to the server for all of the comments for the article, and then, without updating the entire page, inserts the new section for the user to interact with the comments.



### Live Web Pages - How HTML is Updated

Before JavaScript was added, web pages were "Static".

* the web browser just needed to read in the HTML and CSS text files, apply the styles and load the page for display in the browser. 

With JavaScript, we need a way to update the "Live" site with changes.

* new HTML needs to be incorporated into the site.



#### The DOM \(Document Object Model\)

The DOM, or Document Object Model, is an in-memory representation the web browser builds of the HTML document, as it loads the initial HTML page request.

![](../.gitbook/assets/image%20%2818%29.png)

![](../.gitbook/assets/image%20%28163%29.png)

The web browser makes this model accessible to web developers through what is called an API \(Application Programming Interface\), which is just a fancy term to describe the way different software systems communicate with each other programmatically.

Let's say web needed to change the title. The JavaScript code would need to use the DOM API to:

* Find the node in the DOM that needs to be changed
* Update the value for the title

Most changes are much more complex, replacing big chunks of the DOM.

