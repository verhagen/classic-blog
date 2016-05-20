---
layout: post
title: Git Tip - Ignore files and directories for Java development
---


## Introduction

When developing a (Java) project, with git, you mostly do not want all files to end up in the got  project repository. To let git ignore certain 
files and or directories add them to the file `.gitignore`. This file is then added to the git repository, so all developers can use it.


## Action Plan

- Create a file `.gitignore` in the root of the project (working directory). And add rules like to ones below, for a tipical Java project. Here 
  Eclipse, IntelliJ and Maven specific directories will be ignored.

	# Generic
	tmp/
	
	# Maven Configuration
	target/
	
	# Eclipse Configuration
	.settings/
	.classpath
	.project
	
	# IntelliJ Configuration
	.idea/
	*.iml

### Explanation

- Each line starting with an hash `#` are for comments.
- Each line ending with a forward slash `/` will mean it is a directory and all content in the directory should be ignored.
- File or directory names can contain a start `*`, like in the `*.iml` ignore and file with the extension `.iml`.