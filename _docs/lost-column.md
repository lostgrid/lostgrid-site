---
title: "Lost Column"
id: "lost-column"
code-example: "true"
---

<table border="1" style="border-collapse:collapse;width:100%" cellpadding="3" cellspacing="3">
	<tr>
		<td>Table Cell</td>
		<td>Table Cell</td>
	</tr>
	<tr>
		<td>Table Cell</td>
		<td>Table Cell</td>
	</tr>
	<tr>
		<td>Table Cell</td>
		<td>Table Cell</td>
	</tr>
	<tr>
		<td>Table Cell</td>
		<td>Table Cell</td>
	</tr>
	<tr>
		<td>Table Cell</td>
		<td>Table Cell</td>
	</tr>
	<tr>
		<td>Table Cell</td>
		<td>Table Cell</td>
	</tr>
</table>



<ul class="[ list--bare list--rules ]">
    <li>
        <code>fraction</code> This is a simple fraction of the containing element's width.
    </li>
    <li>
        <code>gutter</code> The margin on the right side of the element used to create a gutter. Typically this is left alone and settings.gutter will be used, but you can override it here if you want certain elements to have a particularly large or small gutter (pass 0 for no gutter at all).
        <span class="sub-note">When specifying the gutter, you need to also specify the cycle.</span>
    </li>
    <li>
        <code>cycle</code> Lost works by assigning a margin-right to all elements except the last in the row. It does this by default by using the denominator of the fraction you pick. To override the default use this param., e.g.: .foo { lost-column: 2/4 2; }.
    </li>
    <li>
        <code>flex|no flex</code> Determines whether this element should use Flexbox or not.
    </li>
    <li>
        <code>none</code> Resets the column (back to browser defaults).
    </li>
</ul>

{% highlight css %}
div {
  lost-column: 1/3;
}

div {
  lost-column: 2/6 3 60px flex;
}
{% endhighlight %}
