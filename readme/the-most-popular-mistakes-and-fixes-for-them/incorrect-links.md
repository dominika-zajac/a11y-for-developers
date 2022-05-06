# Incorrect links

Links are a super popular pattern on the internet - very often you want to allow users to navigate between different pages e.g. to check details, learn more, etc. However, even here you should be aware of some potential problems.

First of all, all links should be accessible via keyboard navigation. As long as you are using the custom elements it should be OK, but verify if you don't add e.g. tabindex=-1 or a non-widget role on your custom widget.

Each link should have also a description informing where it navigates. Especially, if you use an icon as a link remember about adding a meaningful label. Or when you use a word `link` check if the context is understandable for the users using the screen readers.&#x20;

The last thing is adding an additional warning when a link is opening in the new tab. It can be implemented in a way that it's visible only to screen reader users. Thanks to that they avoid confusion when trying to come back from opened link to the previous content.

### **Example**

Go to the webpage: [https://dominika-zajac.github.io/a11y-for-developers-examples/incorrect-links/example.html](https://dominika-zajac.github.io/a11y-for-developers-examples/incorrect-links/example.html)

Test the wepage using Lighthouse and Accessibility Insights for web audits. Perform also manual tests - check keyboard navigation and how the content is read by a screen reader.

Note that only 1 problem was found by automated tools - the case where the link has no label at all. However, only 2 links on the page are correct. Can you spot them?

**Answers**: the first and the second links are correct. The first one is correct for displaying links opening in the same tab, the second has a warning visible only for screen reader users about opening in the new tab.&#x20;

The third link has a meaningless description - when you have more links like that on the page it's super hard to know where you'll be redirected after pressing. Especially, when you just "scan" the content or navigate between links on the page.

The fourth one has a missing warning about opening in the new tab. Screen readers' users may be confused and don't know how to go back after using it.

The next one is the only one found by automated tools. The problem here is a completely missing label - so it's hard to say where it goes.

And the last one cannot be reached via keyboard navigation. So people who cannot use a mouse cannot take action using this link.

### Exercise

Do you know how to fix the problems described above? Check if after your changes screen reader is reading the images properly.&#x20;

You can run the code:

* locally from GitHub ([https://github.com/dominika-zajac/a11y-for-developers-examples/tree/main/incorrect-links](https://github.com/dominika-zajac/a11y-for-developers-examples/tree/main/incorrect-links))
* in Stackblitz online editor (note that Lighthouse doesn't work in this setup): [ ](https://stackblitz.com/github/dominika-zajac/a11y-for-developers-examples?file=incorrect-links%2Fexample.html)[https://stackblitz.com/github/dominika-zajac/a11y-for-developers-examples?file=incorrect-links%2Fexample.html](https://stackblitz.com/github/dominika-zajac/a11y-for-developers-examples?file=incorrect-links%2Fexample.html)&#x20;

