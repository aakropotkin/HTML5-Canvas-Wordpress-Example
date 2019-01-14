# Using an HTML5 Canvas element with Wordpress, by Example.

During a recent project I struggled a bit to get an HTML5 Canvas animation I created to display properly in a Wordpress Blog. After arriving at a solution I wanted to create a basic example of the process to share with others.

The body of the provided `post.html` file can be added to a post/page on Wordpress to give the user access to a canvas by embedding it inside of an iframe element.
I found references to this type of solution in several message board posts, but never found a concrete example.
The largest issue I was running into was finding out how to force the script to wait until the document had loaded, because Wordpress prevents the use of `onload` events.
The solution was to use jQuery to trigger my initialization event. Further loading issues can be avoided with the embedded page by building it from scratch with Javascript.
