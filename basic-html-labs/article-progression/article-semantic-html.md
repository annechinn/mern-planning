# Article - Semantic HTML

### Getting Started with the Jelly Fish Article Layout

Our article isn't going to have a top-level header and footer for this draft. We're just going to focus on the article container and its contents.

Adding these semantic elements does nothing to change the way the HTML is displayed on the screen. They are just marking sections of the page with meaning and will enable us to add CSS selectors to eventually style them.

### Changes to Use Semantic Elements

#### Top-level Structure

We can now modify our HTML page to use semantic elements to convey more meaning to the structure of the page. 

```css
<body>
    <main>
        <article>
            <header>
                <!-- Title, Sub-title, Author-->
                <section></section>
                <!-- Video -->
                <section></section>
                <!-- Meet the Jellies -->
                <section></section>
            </header>
            <!-- Pink Jelly -->
            <section>
            </section>
            <!-- Orange Jelly -->
            <section>
            </section>
            <!--Yellow Jelly -->
            <section>
            </section>
        </article>
    </main>
</body>
```

#### Header Section - Title, Sub-title, Author and Date

First, we'll add a few more details to the title section of the page. Notice the addition of the two semantic elements &lt;[address](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/address)&gt; and &lt;[time](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/time)&gt;. 

```markup
<section>
    <p>SCIENCE</p>
    <h1>Jellies From the Deep</h1>
    <p>Tincidunt dui ut ornare lectus venenatis tellus.</p>
    <address>RUBY RAILS</address>
    <time>JANUARY/FEBRUARY 2018</time>
    <hr/>
</section>
```

#### Header Section - Video

```markup
 <section>
    <video controls autoplay muted loop src="videos/jellyfish.mp4"></video>
    <p>Vel quam elementum pulvinar etiam non quam lacus suspendisse. Tincidunt dui ut ornare lectus sit amet
        est placerat in. Lectus nulla at volutpat diam ut venenatis tellus. Sed elementum tempus egestas sed.
        Lectus vestibulum mattis ullamcorper velit sed. Placerat orci nulla pellentesque dignissim enim.
    </p>
</section>
```

#### Header Section - Meet the Jellies Section

Next, we'll add our MEET THE JELLIES section. Notice the replacement of the italics with the  &lt;[address](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/address)&gt; element in each list item for the author byline. 

```markup
<section>
    <h2>MEET THE JELLIES</h2>
    <ul>
        <li>
            <a href="#pink-jelly">The Pink Jelly</a>
            <address>Sally Smith</address>
        </li>
        <li>
            <a href="#orange-jelly">The Orange Jelly</a>
            <address>Dan Dickerson</address>
        </li>
        <li>
            <a href="#yellow-jelly">The Yellow Jelly</a>
            <address>Pam Patterson</address>
        </li>
    </ul>
</section>
```

#### Jellyfish Section

Last, we'll modify the individual jellyfish section to be contained in a &lt;section&gt; element and also use the &lt;[figure](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/figure)&gt;, &lt;[figurecaption](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/figcaption)&gt; and &lt;[address](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/address)&gt; semantic elements to wrap the image. 

The figure and figure caption elements associate an image and its caption, whereas the address element is specifically for marking an author/or byline.

```markup
<section>
    <h3>Pink Jelly</h3>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing
    elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas tellus rutrum tellus
    Tellus rutrum tellus pellentesque eu tincidunt tortor aliquam nulla facilisi. Libero justo laoreet sit amet cursus sit.
    </p>
    <p>Vel quam elementum pulvinar etiam non quam lacus suspendisse. Tincidunt dui ut ornare lectus sit amet
        est placerat in. Lectus nulla at volutpat diam ut  venenatis tellus.
    </p>
    <figure>
        <img src="images/pink-jellyfish.jpg" alt="jellyfish">
        <figcaption><address>Sally Smith</address></figcaption>
    </figure>
</section>
```

### Finished HTML

```markup
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jellies From the Deep</title>
</head>
<body>
    <main>
        <article>
            <header>
                <!------- Title Section -------->
                <section>
                    <p>SCIENCE</p>
                    <h1>Jellies From the Deep</h1>
                    <p>Tincidunt dui ut ornare lectus venenatis tellus.</p>
                    <img src="images/author.png" alt="author">
                    <address>RUBY RAILS</address>
                    <time>JANUARY/FEBRUARY 2018</time>
                    <hr/>
                </section>

                <!------- Video Section -------->
                <section>
                    <video controls autoplay muted loop src="videos/jellyfish.mp4"></video>
                    <p>Vel quam elementum pulvinar etiam non quam lacus suspendisse. Tincidunt dui ut ornare lectus sit amet
                            est placerat in. Lectus nulla at volutpat diam ut venenatis tellus. Sed elementum tempus egestas sed.
                            Lectus vestibulum mattis ullamcorper velit sed. Placerat orci nulla pellentesque dignissim enim.
                    </p>
                </section>

                <!------- Article Index Section -------->
                <section>
                    <h2>MEET THE JELLIES</h2>
                    <ul>
                        <li>
                                <a href="#pink-jelly">The Pink Jelly</a>
                                <address>Sally Smith</address>
                        </li>
                        <li>
                                <a href="#orange-jelly">The Orange Jelly</a>
                                <address>Dan Dickerson</address>
                        </li>
                        <li>
                                <a href="#yellow-jelly">The Yellow Jelly</a>
                                <address>Pam Patterson</address>
                        </li>
                    </ul>
                </section>
            </header>
        
            
            <!--------------------- Pink Jelly ---------------------->
            <section>
                <h3 id="pink-jelly">Pink Jelly</h3>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing
                elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas tellus rutrum tellus
                Tellus rutrum tellus pellentesque eu tincidunt tortor aliquam nulla facilisi. Libero justo laoreet sit amet cursus sit.
                </p>
                <p>Vel quam elementum pulvinar etiam non quam lacus suspendisse. Tincidunt dui ut ornare lectus sit amet
                    est placerat in. Lectus nulla at volutpat diam ut  venenatis tellus.
                </p>
                <figure>
                    <img src="images/pink-jellyfish.jpg" alt="jellyfish">
                    <figcaption><address>Sally Smith</address></figcaption>
                </figure>
            </section>
            
            <!--------------------- Orange Jelly ---------------------->
            <section>
                <h3 id="orange-jelly">Orange Jelly</h3>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing
                    elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas tellus rutrum tellus
                    Tellus rutrum tellus pellentesque eu tincidunt tortor aliquam nulla facilisi. Libero justo laoreet sit amet cursus sit.
                </p>
                <p>Vel quam elementum pulvinar etiam non quam lacus suspendisse. Tincidunt dui ut ornare lectus sit amet
                    est placerat in. Lectus nulla at volutpat diam ut  venenatis tellus.
                </p>
                <figure>
                    <img src="images/orange-jellyfish.jpg" alt="jellyfish">
                    <figcaption><address>Dan Dickerson</address></figcaption>
                </figure>
            </section>
            
            <!--------------------- Yellow Jelly ---------------------->
            <section>
                <h3 id="yellow-jelly">Yellow Jelly</h3>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing
                    elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas tellus rutrum tellus
                    Tellus rutrum tellus pellentesque eu tincidunt tortor aliquam nulla facilisi. Libero justo laoreet sit amet cursus sit.
                </p>
                <p>Vel quam elementum pulvinar etiam non quam lacus suspendisse. Tincidunt dui ut ornare lectus sit amet
                    est placerat in. Lectus nulla at volutpat diam ut  venenatis tellus.
                </p>
                <figure>
                    <img src="images/yellow-jellyfish.jpg" alt="jellyfish">
                    <figcaption><address>Pam Patterson</address></figcaption>
                </figure>
            </section>
        </article>
    </main>
</body>
</html>
<body>
```

### Assignment

Check-in your changes and push them to GitHub, then I will check them off to make sure they've all been completed.

* git add -a .
* got commit -m""
* git push

