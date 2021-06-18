# How a Web Page Gets Loaded

The high-level steps the browser takes when you enter an URL into the search input box are the following:

1. Enter a URL into a web browser
2. Browser looks up the IP address for the domain name via DNS.
3. Browser sends a HTTP request to the server.
4. Server sends back a HTTP response.
5. Browser begins rendering the HTML.
6. Browser sends requests for additional objects embedded in HTML \(images, CSS, JavaScript\) and repeats steps 3-5.
7. Once the page is loaded, the browser sends further asynchronous requests as needed.

Step 5-6: The web browser reads through and and parses the HTML text file line-by-line. As it encounters references to external files, it will send additional requests to the server for each one.

* Stylesheets
* Fonts
* JavaScript files
* Images

![](../.gitbook/assets/image%20%2836%29.png)

Below is an example of what references to external files within an HTML document might look like. 

```markup
<!DOCTYPE html>
<html lang="en">
<head>
    <link rel="stylesheet" href="./scripts/styles.css">
    <title>Document</title>
</head>
<body>
    <header></header>
    <main>
        <img src="./images/profile.jpg" />
    </main>
    <footer></footer>
    
    <script src="./scripts/bundle.js"></script>
</body>
</html>

```

### Bundling Files on the Server for Efficient Delivery

It is now common for the process of preparing a web site for delivery to bundle files of the same type into a single package. For example, all of the JavaScript files would reside in a single package and all of the CSS files would reside in a separate package. 

![](../.gitbook/assets/image%20%2862%29.png)

### Anatomy of a Page Request/Response

The image below shows the Request and Response taken from the Chrome Developer Tools when inspecting the Network traffic after the URL csszengarden.com is entered into the search input box of the browser.

#### Default HTML Page - Request/Response

As you can see, the request asks for \(Request Method: GET\) some data from the web server for the given URL.

![](../.gitbook/assets/image%20%28124%29.png)

The web server responds with the contents of the default HTML document for the site. Looking at the line highlighted in red, you can see a request for the stylesheet file "/214/214.css". A request will be made to the web server for this file next.

#### CSS File - Request Response

The web server next makes another request for the CSS file and gets back the contents of that files in the response. 

![](../.gitbook/assets/image%20%28158%29.png)

