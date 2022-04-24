# Missing alternative text

Sometimes it’s hard to understand something without additional information. It’s why we have footnotes in books or cards with item descriptions in museums. The same story may occur on your site — especially if we remove their visual part. Add alternative text to your images by using an `alt` tag for images or the correct title in SVG elements. Thanks to that also people using screen readers will know what is in the picture. When the image is only decorative leave those tags empty or add `aria-hidden=true`— screen readers will understand and omit that. Also, check if without visual content all interactive elements are still well-labeled— tags like `aria-label`, `aria-labelledby`, `aria-description` or `aria-describedby` might be super useful in that case.



When to use the given tags?

* **aria-label** => when you want to add a short description of an image/element and provide a string as a value
* **aria-labelledby** => when you want to add a short description of an image/element and provide the ID of another element as a value&#x20;
* **aria-description** => when you want to add additional, longer information for an element and provide a string with a description as a value
* **aria-describedby** => when you want to add additional, longer information for an element and provide the ID of another element as a value&#x20;
* **aria-hidden** => when an element is only decorative and should be ignored by a screen reader
* **alt** => on img HTML element when you provide string describing the picture
* **title** => inside svg HTML element when you provide string describing the picture

**Note:** If your page supports multilanguage, also alternative texts should be translated!
