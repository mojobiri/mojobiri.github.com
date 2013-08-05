---
layout: post
title:  "Exception handling in small methods."
categories:
excerpt: Ruby quick tip for beginners.
tags: rubyquicktip
---

Ruby quick tip for beginners.

You can use keywords **rescue**, **else**, **ensure** in methods without **begin**, **end**. Usefull in short methods.

{% highlight ruby %}
def method_name(x)
    rescue 
        # exception handle
    else 
        # do something if no exception occured
    ensure 
        # do something anyway
end
{% endhighlight %}

equal to

{% highlight ruby %}
def method_name(x)
    begin
        rescue 
            # exception handle
        else 
            # do something if no exception occured
        ensure 
            # do something anyway
    end
end
{% endhighlight %}