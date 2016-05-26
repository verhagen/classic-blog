---
layout: post
title: Eclipse Tip - Java Template - Simple Logging Facade for Java (slf4j)
---
Create a Java editor template for creating a slf4j logger instance.


## Action Plan

### Create a New Java Template

- Open Eclipse Preferences
- Select from the tree on the left _Java > Editor > Templates_
- Use the button __New ...__, to create a new template
- The dialog _New Template_ will open
- Add the _name_ field __logger__, this is name which is used in the Java Editor, when referring to this template
- Select the type of _content_, this one is of type __Java__ 
- Fill in a meaningful _description_ like __Create a slf4j logging instance__
- Add the _Pattern_ as show below

{% highlight java %}
private static Logger logger = LoggerFactory.getLogger(${enclosing_type}.class);
${:import(org.slf4j.Logger, org.slf4j.LoggerFactory)}
{% endhighlight %}

![Eclipse Preferences]({{ site.url }}/images/eclipse/eclipse-preferences-java-template-slf4j-01.jpeg)

- Press button __OK__ to close the dialog

![Eclipse Preferences]({{ site.url }}/images/eclipse/eclipse-preferences-java-template-slf4j-00.jpeg)


### Use the Logger Template

- Open a Java class
- Go to the location where you want to declare the logging instance
- On a new line enter __logg__ and press &lt;ctrl&gt;-&lt;space&gt; to see code suggestions

![Eclipse Preferences]({{ site.url }}/images/eclipse/eclipse-preferences-java-template-slf4j-02.jpeg)

- From the list select the _logger_ template
- Now a new line with the logger instance should be there, including the required imports

{% highlight java %}
import org.slf4j.Logger;
import org.slf4j.LoggerFactory;

public class Project {
    private static Logger logger = LoggerFactory.getLogger(Project.class);

}
{% endhighlight %}


### Export Java Templates


### Import Java Templates

