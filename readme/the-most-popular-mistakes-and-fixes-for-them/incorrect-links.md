# Incorrect links

Links are a super popular pattern on the internet - very often you want to allow users to navigate between different pages e.g. to check details, learn more, etc. However, even here you should be aware of some potential problems.

First of all, all links should be accessible via keyboard navigation. As long as you are using the custom elements it should be OK, but verify if you don't add e.g. tabindex=-1 or a non-widget role on your custom widget.

Each link should have also a description informing where it navigates. Especially, if you use an icon as a link remember about adding a meaningful label. Or when you use a word `link` check if the context is understandable for the users using the screen readers.&#x20;

The last thing is adding an additional warning when a link is opening in the new tab. It can be implemented in a way that it's visible only to screen reader users. Thanks to that they avoid confusion when trying to come back from opened link to the previous content.
