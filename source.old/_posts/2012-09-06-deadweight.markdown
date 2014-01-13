---
layout: post
title: "Deadweight"
date: 2012-09-06 15:36
comments: false
external-url: https://github.com/aanand/deadweight
---
{% blockquote %}
Deadweight is a CSS coverage tool. Given a set of stylesheets and a set of URLs, it determines which selectors are actually used and reports which can be "safely" deleted.

``` sh How to Use It
$ deadweight -s styles.css -s ie.css index.html about.html
$ deadweight -s http://www.tigerbloodwins.com/index.css http://www.tigerbloodwins.com/
$ deadweight --root http://kottke.org/ -s '/templates/2009/css.php?p=mac' / /everfresh /about
```
{% endblockquote %}

Using this for a few minutes will really clean up your stylsheets.

Via [Mr. Mann Merlin Mann](http://www.kungfugrippe.com/post/31002931568) Way of the future