---
title: "anonymity"
bg: '#63BD2F'
color: white
fa-icon: user-secret
---

Algorithm of Location K-anonymity

{% highlight text linenos=table %}

node = FindNode(Location);
repeat
  if the number of moving objects in node > K then
     break;
  end
  node = ExtendASR(node);
until node is the entire space U;
return node;

{% endhighlight %}



