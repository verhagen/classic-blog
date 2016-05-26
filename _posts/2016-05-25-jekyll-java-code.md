---
layout: post
title: Sample Java Code in Jekyll
---
Show some Java code example in Jekyll based site.

<kbd>CTRL</kbd>+<kbd>Z</kbd>

{% highlight java %}
package org.organisation.project;

import org.slf4j.Logger;
import org.slf4j.LoggerFactory;

/**
 * This application...
 */
public class Application {
	// Logger instance
	private static Logger logger = LoggerFactory.getLogger(Project.class);

	/**
	 * @param args - the argument to startup the applicaiton
	 */
	public static void main(String[] args) {
		/*
		 * Multi line comment.
		 */
		System.out.println("Some text");
		char c = 'x';
		int i = 100;
	}

}
{% endhighlight %}

