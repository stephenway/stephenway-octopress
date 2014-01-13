---
layout: post
title: "position: sticky;"
date: 2012-09-02 10:00
comments: false
external-url: http://updates.html5rocks.com/2012/08/Stick-your-landings-position-sticky-lands-in-WebKit
---
Eric Bidelman shows us a little hidden gem in the latest Webkit Nightly and Chrome Canary.

{% blockquote %}
By simply adding position: sticky (vendor prefixed), we can tell an element to be position: relative until the user scrolls the item (or its parent) to be 15px from the top:

``` css
.sticky {
  position: -webkit-sticky;
  position: -moz-sticky;
  position: -ms-sticky;
  position: -o-sticky;
  top: 15px;
}
```
{% endblockquote %}

I recently did a theme that uses this functionality with a navigation bar, it would have been really nice to have this position type available instead of a JS solution which proved to complicate a few things down the road.