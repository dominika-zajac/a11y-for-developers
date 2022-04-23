# Jest-axe unit tests

If we can unit test our components to be sure they work and display as expected, why don’t we unit test them against accessibility problems? Yes, it’s possible. One of the packages you can use is `jest-axe`. The unit test for accessibility may look like the snippet below (taken from jest-axe readme file). Of course, you can also set a list of your rules to include/exclude both globally and just for the given test.

{% embed url="https://gist.github.com/dominika-zajac/59035f2120081a1a804a91173910369b" %}
Example of jest-axe a11y unit test
{% endembed %}

You can find more examples and information about the tool on its GitHub page: [https://github.com/nickcolley/jest-axe](https://github.com/nickcolley/jest-axe)
