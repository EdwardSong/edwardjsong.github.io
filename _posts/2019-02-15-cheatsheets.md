---
layout: default
title: My OpenSAML SSO Implementation Notes
tags: [OpenSAML, SAML, SSO]
permalink: /saml
category: SSO, SAML
---

# Cheat sheets

## Table of Contents

### OS/X
* Show Hidden Files in Finder
  *  `Command + Shift + .`--ta2019

### IntelliJ
* Plugins
    * Archive browser - view contents of archive files (.jar, .war, .zip) 

### Docker
* Install Docker on a mac (Docker for mac) which does not require a virtual box
    * `brew cask install docker`
* Build a docker image
    * `docker build --tag 20190314 .`

### Gradle
<pre>
/* Enables jar to be created when war plugin is applied.
   When the war plugin is applied the default behaviour is to skip the jar task.
*/
jar {
   enabled = true
}
</pre>
    
## Authentication Flow


[back](./)