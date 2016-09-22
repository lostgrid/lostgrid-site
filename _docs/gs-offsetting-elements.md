---
order: 5
title: "Offsetting Elements"
nav: "offsetting-elements"
code-example: "true"
type: "getting-started"
description: "You can offset columns easily. To offset in the other direction, pass a negative fraction."

---

{% highlight html %}
<section>
  <div>1</div>
  <div>2</div>
</section>
{% endhighlight %}

{% highlight css %}
div {
  lost-column: 1/3;
}

div:first-child {
  lost-offset: 1/3;
}
{% endhighlight %}

**Note: This is presently reversed from typical behavior due to initial API and the need to retain the API. Version 8 is planning to implement this in a more natural way.**
