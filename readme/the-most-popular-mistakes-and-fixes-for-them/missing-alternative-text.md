# Missing alternative text

### Intro

Sometimes it’s hard to understand something without additional information. It’s why we have footnotes in books or cards with item descriptions in museums. The same story may occur on your site — especially if we remove their visual part. Add alternative text to your images by using an `alt` tag for images or the correct title in SVG elements. Thanks to that also people using screen readers will know what is in the picture. When the image is only decorative leave those tags empty or add `aria-hidden=true`— screen readers will understand and omit that. Also, check if without visual content all interactive elements are still well-labeled— tags like `aria-label`, `aria-labelledby`, `aria-description` or `aria-describedby` might be super useful in that case.

### When to use the given tags?

* **aria-label** => when you want to add a short description of an image/element and provide a string as a value
* **aria-labelledby** => when you want to add a short description of an image/element and provide the ID of another element as a value&#x20;
* **aria-description** => when you want to add additional, longer information for an element and provide a string with a description as a value
* **aria-describedby** => when you want to add additional, longer information for an element and provide the ID of another element as a value&#x20;
* **aria-hidden** or empty => when an element is only decorative and should be ignored by a screen reader
* **alt** => on img HTML element when you provide string describing the picture
* **title** => inside svg HTML element when you provide string describing the picture

**Note:** If your page supports multilanguage, also alternative texts should be translated!

### **Example**

Go to webpage: [https://dominika-zajac.github.io/a11y-for-developers-examples/text-alternative/incorrect-examples.html](https://dominika-zajac.github.io/a11y-for-developers-examples/text-alternative/incorrect-examples.html)

Try to read the page with your screen reader. It would be impossible to understand the content of images without seeing them, wouldn't it? Let's check what is happening here.

On the page you can find 4 images presenting popular mistakes with alternative text:

* missing alt text
* the empty string provided as alt text
* the ID of the element provided as a value in the aria-label
* incorrect ID provided as a value in the aria-labelledby property.

Check the page with Lighthouse or Accessibility Insights for Web audits (You can learn how to do so in other sections of my tutorial: [Lighthouse](../useful-tools/lighthouse-audits.md) and [Accessibility Insights for Web](../useful-tools/web-insights-for-web.md)).&#x20;

The report should look similar to the screenshots below and informs about problems with aria labels.



Report from Lighthouse:

![Example of a report from Lighthouse with info about problems with an alternative textnananana](<../../.gitbook/assets/image (3) (1) (1) (1).png>)

Report from Accessibility Insights for Web:

![5 images of a bunny in front of the computer. The first, third, and fifth items have a red border and exclamation mark in the top right corner.](<../../.gitbook/assets/image (1) (1).png>)

![Example of a report from Accessibility Insights for web with info about problems with an alternative text](<../../.gitbook/assets/image (5) (1) (1).png>)

Notice that **only 3 of 5 problems were found by automated tools**. Why? Because an empty string as a value in alt property can be proper - in a case when the image is only decorative and should be ignored by screen readers. Also, the ID of another element in aria-label cannot be detected by an automated tool - it will be just read as it is for a user. It's why we need to perform manual tests!

### Exercise

Do you know how to fix the problems described above? Check if after your changes screen reader is reading the images properly.&#x20;

You can run the code:

* locally from GitHub ([https://github.com/dominika-zajac/a11y-for-developers-examples/tree/main/text-alternative](https://github.com/dominika-zajac/a11y-for-developers-examples/tree/main/text-alternative))
* in Stackblitz online editor (note that Lighthouse doesn't work in this setup): [https://stackblitz.com/github/dominika-zajac/a11y-for-developers-examples?file=text-alternative%2Fincorrect-examples.html](https://stackblitz.com/github/dominika-zajac/a11y-for-developers-examples?file=text-alternative%2Fincorrect-examples.html)&#x20;





