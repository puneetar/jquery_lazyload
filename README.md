Lazy Load Plugin for jQuery
Lazy Load delays loading of images in long web pages. Images outside of viewport wont be loaded before user scrolls to them. This is opposite of image preloading.

Using Lazy Load on long web pages containing many large images makes the page load faster. Browser will be in ready state after loading visible images. In some cases it can also help to reduce server load.

Lazy Load is inspired by YUI ImageLoader Utility by Matt Mlinac.

How to Use?

Lazy Load depends on jQuery. Include them both in end of your HTML code:

<script src="jquery.js" type="text/javascript"></script>
<script src="jquery.lazyload.js" type="text/javascript"></script>
You must alter your HTML code. URL of the real image must be put into data-original attribute. It is good idea to give Lazy Loaded image a specific class. This way you can easily control which images plugin is binded to. Note that you should have width and height attributes in your image tag.

<img class="lazy" data-original="img/example.jpg" width="640" height="480">
then in your code do:

$("img.lazy").lazyload();
This causes all images of class lazy to be lazy loaded.

More information on Lazy Load project page.
