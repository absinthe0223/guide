Wordpress Best Practices
========================

Working in Wordpress, it’s important that we do our work in a clean,
maintainable, model. As such, following a few simple rules and best practices
will help ensure that we don’t make a mistake (that we’ve likely already made
and had to fix).  Let’s just make NEW mistakes.

-   **DO** Create a custom.css file for your custom css.

-   **DON’T** Edit any theme or child theme style sheets (unless absolutely
    necessary).  Put all your CSS in a separate CSS file, and then if you must,
    link this into the original theme’s CSS file. This way, you can upgrade the
    child theme without losing all your code changes.

-   **DO **Build any “widget” or item in the front end that clients will use,
    levering ONLY the GUI and UI editor. Then,modify this code using a CSS class
    or ID attribute in your custom.css file to give the widget or area the
    desired behavior.

-   **DO** Link to images using the image editor.  This is critical as when you
    embed FULL URLs in the code, when you push to production, we will then have
    to go through and rewrite URLs, which is a huge time suck.

 
