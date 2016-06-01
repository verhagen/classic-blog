---
layout: post
title: Git Tip - Ignore Specific Files and Directories
---

When developing a (Java) project, you mostly do not want all files to end up in the git repository. To let git ignore certain 
files and / or hole directories, add them to the file `.gitignore`. This file is then added to the git repository, so all
developers can use it.

Typical files that should not end up in a git repository, are configuration files of tools used during development. For Java projects these are tipical Eclipse configuration, IntelliJ configuration and the Maven `target` directory.


## Action Plan

- Create a file `.gitignore` in the root of the project (working directory). And add rules like to ones below, for a typical
Java project. Here Eclipse, IntelliJ and Maven specific directories will be ignored.

{% highlight plain text %}
# Generic
tmp/

# Maven Configuration
target/
pom.xml.tag
pom.xml.releaseBackup
pom.xml.next
release.properties

# Eclipse Configuration
.settings/
.classpath
.project

# IntelliJ Configuration
.idea/
*.iml
{% endhighlight %}


### Explanation

- Each line starting with an hash `#` are for comments.
- Each line ending with a forward slash `/` will mean it is a directory and all content in the directory should be ignored.
- File or directory names can contain a start `*`, like in the `*.iml` ignore and file with the extension `.iml`.