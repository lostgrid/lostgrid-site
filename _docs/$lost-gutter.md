---
title: "Lost Gutter"
nav: "lost-gutter"
code-example: "true"
type: "variable"
description: "Align nested elements. Apply this to a parent container."
rules:
  - rule: "flex | no-flex"
    description: "Determines whether this element should use Flexbox or not."
---

{% highlight css %}
.parent {
  lost-align: right;
  width: 600px;
  height: 400px;
}

.child {
  width: 300px;
  height: 150px;
}
{% endhighlight %}
