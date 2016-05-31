---
layout: post
title: Eclipse Tip - Add Maven Archetypes Catalog
---
When an Archetype is not found, through the default defined Archetype catalogs, you can add an
additional remote or local catalog.


## Action Plan

### Create a New Java Template

- Open Eclipse Preferences
- Select from the tree on the left _Maven > Archetypes_  
![Eclipse Preferences]({{ site.url }}/images/eclipse/eclipse-preferences-maven-archetypes-00.jpg)
- Use the button _Add Remote Catalog..._
- The dialog _Remote Archetype Catalog_ will open
- Fill in the field _Catalog File_: __https://repo1.maven.org/maven2/archetype-catalog.xml__
- Fill in the field _Description_: __Maven 2 Archetypes__
- Use the button _Verify..._ to see if the catalog can be found  
  At the top, should appear how many archetypes where found
- Use the button _OK_ to close the dialog
- Use the button _OK_ to close the dialog _Preferences_
