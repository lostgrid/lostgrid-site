---
title: "Lost Offset"
nav: "lost-offset"
code-example: "true"
type: "property-option"
description: "Margin to the left, right, bottom, or top, of an element depending on if the fraction passed is positive or negative. It works for both horizontal and vertical grids but not both."
rules:
  - rule: "fraction"
    description: "Fraction of the container to be offset."
  - rule: "row | column"
    description: "Direction the grid is going. Should be the opposite of the column or row it's being used on. Defaults to row."
    sub-note: "Negative numbers for right offsets, positive numbers for left offsets."
  - rule: "gutter"
    description: "How large the gutter involved is, typically this won't be adjusted, but if you have set the elements for that container to have different gutters than default, you will need to match that gutter here as well."
---

**Note: This is presently reversed from typical behavior due to initial API and the need to retain the API. Version 8 is planning to implement this in a more natural way.**

{% highlight css %}
.two-elements {
  lost-column: 1/3;
}

.two-elements:first-child {
  lost-offset: 1/3;
}
{% endhighlight %}
