# html-click-js

A plugin to handle all click interactions with custom attributes in HTML

- Already included in [HTML-Skinning-Boilerplate](https://github.com/kamlekar/HTML-Skinning-Boilerplate/tree/master/site/assets/libs)

##Docs:

- `html-click.js` will work when an element has `html-click` class.

###Custom Attributes:

- `data-html-class` : The value of this custom attribute will be added as class to the clicked element or targeted element (_targeted using `data-html-target`_). If this attribute is not present, the default value is taken which is "active" class.
- `data-html-target`: The value of this custom attribute represents css selector to fetch the targeted element to which the `data-html-class` value must be added as class. This attribute is optional. When this attribute is not mentioned, the targeted element will be the self element which is clicked.
- `data-html-toggle`: This attribute value determines whether the click Interaction should act as toggle or add class or remove class. Possible values are "toggle"(_default_), "add" and "remove". This attribute is optional.
- `data-html-outside-click`: This attribute value determines whether this element with `html-class` class name should move to default state when clicked outside of this element. For example, if there is a `div.html-click` element which has custom attributes like `data-html-toggle="toggle"` and `data-html-outside-click="true"`. When user clicks on this element, `active` class is added to this element. When user clicks outside of this element, the `active` will be removed (_the element goes to default state_).


