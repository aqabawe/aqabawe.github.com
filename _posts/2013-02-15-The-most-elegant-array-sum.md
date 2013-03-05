---
layout: post
title: The Most Elegant Ruby Array Sum
description: Ruby inject sum array or array arthimatic operations
keywords: ruby,rails,ruby bites,mamoun,saudi,aqabawe, inject, array sum
---

<p>
Ruby is an elegant language, it's <a href='http://en.wikipedia.org/wiki/Syntactic_sugar'>syntactic sugar</a> is one of the most pleasing to the programmer's eyes, and makes it very easy to go over code and understand it's function in a glimpse.
<p>
<p>
Below is a prime example of that syntactic sugar, this is array sum done in an elegant way:
</p>
{% highlight ruby %}
  > [1, 2, 10].inject(:+)
  => 13

  > ['A', 'B', 'B', 'A'].inject(:+)
  => "ABBA"

{% endhighlight %}

<p>
You can use reduce instead of inject if you prefer, and you can use any binary operator in the same way:
</p>

{% highlight ruby %}
 > [2, 2, 10].reduce(:*)
 => 40

 # Remove floating point if you want integer division

 > [2.0, 2.0, 10.0].inject(:/)
 => 0.1
{% endhighlight %}
