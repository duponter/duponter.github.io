---
layout: post
title: Java Function Flowchart
comments: True
---

Once in three Java SE versions, a major one is released, with either lots of new classes, like the introduction of the Collections API in Java 2 or syntactic changes, when Java 5 introduced Generics. Java 8 SE, however, introduces both with a new Streams API and a renewed DateTime API and syntax changes with the lambda expressions and method references. To keep up with all these changes, one has to do a lot of reading and, of course, experimenting.

Java 8 introduces a new package <a href="http://docs.oracle.com/javase/8/docs/api/java/util/function/package-summary.html" target="_blank">java.util.function</a> which contains 43 new Functional Interfaces to target lamba expressions and method references.

As with the Collections API in Java 2, a flowchart existed to choose the best fitting implementation.

### Images

Basic Flow
![Basic Flow](/public/img/2014/08/15/function-flowchart/java8_function_flowchart_basic.jpg "Basic Java 8 Function Flowchart")

Extended Flow
![Extended Flow](/public/img/2014/08/15/function-flowchart/java8_function_flowchart_extended.jpg "Extended Java 8 Function Flowchart")

### Code

Some tips about the usage of UnaryOperator:

{% highlight java %}
private Function<String, String> chainable;
private UnaryOperator<String> unchainable;
{% endhighlight %}

### Gists via GitHub Pages
{% gist d2d8eb2cac83eef45d69 %}
