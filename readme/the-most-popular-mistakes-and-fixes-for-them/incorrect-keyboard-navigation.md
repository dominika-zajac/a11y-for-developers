# Incorrect keyboard navigation

As you may remember from the [Why you should think about accessibility](../why-you-should-think-about-accessibility.md) section, many people are using assistive tools like special keyboards or screen readers to use the Internet. Unfortunately, many webpages are not ready for that - also, problems with incorrect keyboard navigation are mostly not found by automated tools. So what is worth checking?

First of all, check if **all interactive elements can be reached via keyboard**. Use `Tab` to navigate between elements. Use Tab + Shift to go to the previous element.&#x20;

Check how elements like **modals or popovers** behave. Where is the focus when you open them? And where it is after close? It should move to the popup/modal after opening and come back to the element which triggered opening after the close. Without that users may be lost in navigation.

It's also worth checking **the custom widgets/elements**. Using build-in HTML elements like buttons or input will provide some support - when you use your styled elements you should probably implement support for navigation by yourself.

Special treatment is needed also in **lists**. As they can be very long we don't want users to navigate between the list items with tabs. The desired behavior is:

* the first tab goes to the first element of the list
* next tabs navigate between elements on this list item
* the last one goes outside the list, to the next focusable element.

If you want to go from the first list item to the next one (or to the previous one), you should use arrow keys for that.

A common pattern is also **providing some shortcuts** to help with navigation e.g. pressing F6 should jump to the next section and F6+Shift to the previous. On Mac computers, it's sometimes F6+Cmd and F6+Cmd+Shift respectively.

Another topic is about things that **shouldn't happen** on navigation. Typical actions like clicking the Tab should not trigger any unexpected actions like sending the form.&#x20;

The last comment, mostly connected with usability, is **the number of clicks/presses needed to navigate** through the content. If you need to press Tab 20 times to reach the main article on the page, you should probably reconsider your structure, provide the link to skip the navigation or implement some shortcuts.&#x20;

### **Example**

****

### **Excercise**

Can you fix navigation problems from the example mentioned above? You can run the code:

* locally from GitHub ([https://github.com/dominika-zajac/a11y-for-developers-examples/tree/main/text-alternative](https://github.com/dominika-zajac/a11y-for-developers-examples/tree/main/text-alternative))
* in Stackblitz online editor (note that Lighthouse doesn't work in this setup): [https://stackblitz.com/github/dominika-zajac/a11y-for-developers-examples?file=text-alternative%2Fincorrect-examples.html](https://stackblitz.com/github/dominika-zajac/a11y-for-developers-examples?file=text-alternative%2Fincorrect-examples.html)&#x20;
