# Chrome Dev Tools - Intro

### Enter [internetingishard.com](https://www.internetingishard.com/) in browser search box

![](../.gitbook/assets/image%20%2823%29.png)

### Launch Chrome Developer Tools

Bring up the context-menu and select the "Inspect" menu option, or Ctrl-Shift-I on Windows

### Network Tab

When you enter an URL \(Uniform Resource Locator\) into the browser search input box, a lot of communication is going on behind the scenes between the web browser and the web server to retrieve the collection of files that are necessary to fully display the web page. There is the top-level HTML page, but also stylesheets, JavaScript files, fonts, images, videos, and more. 

After the web browser receives the response for the initial HTML page, it will read through and sequentially request any files required that it encounters within the HTML markup.

This exercise walks you through the using the Chrome Browser Development Tools, and specifically the Network View, to see the details of these requests.

### Click on the Network tab

It is showing all of the files that are being requested from the web server when we requested the URL, internetingishard.com. The first request is for internetingishard.com, followed by requests for a stylesheet, image, and JavaScript file.

![](../.gitbook/assets/image%20%28122%29.png)

**Network view:** 

**Request Headers:** If you click on the Headers tab on the low right with the first request selected, you can see the details of the request, including the Request URL, The Request Method of GET, which means it is requesting data from the server, and the IP Address that it has resolved through DNS for the server.

![](../.gitbook/assets/image%20%28143%29.png)

**Response:** Below, the view on the right has been switched from Headers to  Response, and now we can see what the web server is returning for the request. It is the default HTML page for the site.

If you look within the &lt;head&gt; element in the Response, you can see the &lt;link&gt; element for the stylesheet and following the blue arrow, you can see that it is the next file that the browser makes a request for.

![](../.gitbook/assets/image%20%28167%29.png)

**Questions**

In the previous screenshot we can see where the stylesheet file is included in the returned HTML. Can you find where the script file named  "**global-466310.js"** is included in the file?   Any ideas why it is included at the end?

Can you find the network IP address for the GET request to internetingishard.com?

### Other Tabs

![](../.gitbook/assets/image%20%287%29.png)

**Live HTML Document** - This is the current rendering of the page.

**DOM - HTML** - The DOM is displayed, allowing you to view the entire hierarchical structure representing the live version of the page. For example, if JavaScript was used to add a new section to the DOM, that section would be included. The developer can hide, add, or modify any of the HTML displayed.

**DOM - CSS** - The DOM  also displays a representation of all of the CSS that has been included for the page, and how the CSS is being applied to the page elements. The developer can add/modify any of these settings.

Web developers use this interface for testing and debugging their web pages. They can try out changes quickly without having to change their source code. The Chrome Developer Tools will be one of the most useful tools you will learn and become part of your daily work.

