# Insufficient color contrast ratio

Insufficient color contrast ratio is one of the most popular problems connected with accessibility. Fortunately, it is quite well found by automated tools like Lighthouse or Accessibility Insights for Web. But did you know that Chrome DevTools can help you not only detect that issue but also fix it? How to do so?

![](https://res.cloudinary.com/practicaldev/image/fetch/s--YuvV-hBM--/c\_limit%2Cf\_auto%2Cfl\_progressive%2Cq\_auto%2Cw\_880/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/tsvaq7spm996wodbam8f.png)

When you open Chrome DevTools and inspect the given element toolbar details of it will be presented. And as it’s visible on the picture it may show us an orange warning icon close to the Contrast category. It means the contrast color ratio between text on that element and its background is not sufficient.

![](https://res.cloudinary.com/practicaldev/image/fetch/s--xCA9fZCP--/c\_limit%2Cf\_auto%2Cfl\_progressive%2Cq\_auto%2Cw\_880/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/21lc6rqxr1zsi92hhyq9.png)

When you take a look at the Styles tab of that element you can do even more. Click on the square color preview on the left side of the color property value to open the color picker. Below the color value input, you may see an expendable section with contrast ratio information. The red icon close to the ratio informs us that we should take a look at that values. And reload button allows Chrome to automatically propose the new color — which will have a correct contrast ratio and as close to ours as possible. Nice way to fix that issue, don’t you think?

