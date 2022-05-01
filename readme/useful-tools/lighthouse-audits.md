# Lighthouse audits

Many developers (especially tech newbies) tell me they know the basics, they feel accessibility is important but they don’t know where to start. This is where automatic audits may help. The easiest way to perform an accessibility audit on your webpage is just to use a tool already built-in into the Chrome browser — Chrome DevTools. Just:

* Use ctrl + shift + I on Linux/Windows or cmd + shift + I on Mac to open the panel,
* Go to the `Lighthouse` tab,
* Tick `Accessibility` checkbox,
* Decide which version (desktop or mobile) you want to test,
* Click the`Generate Raport`button.

After some seconds you will receive the report (like in the picture below) with the most important data.

![Example report after performing accessibility audit in Chrome DevTools](<../../.gitbook/assets/image (1) (1) (1).png>)



OK, so what have we got here? First of all, our webpage is scored on a scale of 1–100. A score below 50 is considered bad, 51–89 medium and 90–100 is the score we want to achieve. But the number is not all. The most important thing in that audit is the list of failing audits — visible just below the main score. When you click on one of the audits and expend details, you will receive much more data — e.g. a link to an article where you can learn more about a given problem and a list of failing elements. What’s more — when you click on the failing element you will be redirected to it in the `Source` tab where you can find more info about the element and where you can play with its CSS or attributes. Definitely worth checking!

![Example of problem detected with the Lighthouse audit](<../../.gitbook/assets/image (3) (1) (1) (1) (1).png>)

Personally, I strongly recommend checking not only the section with failed audits but also the passed ones — thanks to that you can learn what is important and improve your skills.
