---
layout: post
title:  "metaprogramming on ruby, part 1"
date:   2015-12-26 10:28:00
categories: ruby
---

a quick reminder about the ruby classes and the instances, how to idenfity them

{% highlight ruby %}

class MyClass
  def my_method
    @v = 1
  end
end

obj = MyClass.new
obj.class # => MyClass
obj.my_method

obj.instance_variables # => [:@v]
obj.instance_methods == "abc".methods #true
obj.superclass
obj.ancestors
obj.methods.grep(/my/) # => [:my_method]
{% endhighlight %}
