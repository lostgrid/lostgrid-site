---
title: "Lost Move"
nav: "lost-move"
code-example: "true"
type: "property-option"
description: "Source ordering. Shift elements left, right, up, or down, by their left or top position by passing a positive or negative fraction."
rules:
  - rule: "fraction"
    description: "Fraction of the container to be shifted."
  - rule: "row|column"
    description: "Direction the grid is going. Should be the opposite of the column or row it's being used on."
  - rule: "gutter"
    description: "Adjust the size of the gutter for this movement. Should match the element's gutter."
---

**If a gutter is set, lost-move will not retain it and will need to be set manually.** See [#195](https://github.com/peterramsing/lost/issues/195) for more details.

{% highlight css %}
div {
  lost-column: 1/2;
}

div:first-child {
  lost-move: 1/2;
}

div:last-child {
  lost-move: -1/2;
}
{% endhighlight %}

{% highlight css %}
div {
  lost-column: 1/2 0 0;
}

div:first-child {
  lost-move: 1/2 0 0;
}

div:last-child {
  lost-move: -1/2 0 0;
}
{% endhighlight %}
