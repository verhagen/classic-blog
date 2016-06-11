---
layout: post
title: Maven Tip - Source and Output Encoding UTF-8
tags: [maven, tip]
---
Add the properties `project.build.sourceEncoding` and `project.reporting.outputEncoding` with the value `UTF-8` to the `properties` entry.


# Setting the Source and Output Encoding to UTF-8

{% highlight plain text %}
	<properties>
		<project.build.sourceEncoding>UTF-8</project.build.sourceEncoding>
	    <project.reporting.outputEncoding>UTF-8</project.reporting.outputEncoding>

		...
	</properties>
{% endhighlight %}
