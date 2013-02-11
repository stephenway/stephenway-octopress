---
layout: post
title: "A Simple Progress Bar"
date: 2012-09-07 17:44
comments: false
external-url: http://playground.deaxon.com/css/progress-bar/
---
This is an impressive use of CSS applied to just one HTML progress tag.

{% codeblock lang:css %}
@-webkit-keyframes m {
  0% {background-position:20px 0} 100% {}
}
@-moz-keyframes m {
  0% {background-position:20px 0} 100% {background-position:0 0}
}
body {
  background:rgb(235,235,240);
}
progress {
  position:absolute;
  left:50%;
  top:50%;
  margin:-20px 0 0 -31px;
  width:62px;
  height:12px;
  border:1px solid rgb(160,170,190);
  border-radius:6px;
  background:
    -webkit-radial-gradient(rgba(140,153,172,.3), rgba(140,153,172,0)),
    -webkit-linear-gradient(
      #fff 15%, #e9ecf1 15%, #d2d9e1 50%, #bdc6d2 50%, #dfe7ed
    );
  background:
    -moz-radial-gradient(rgba(140,153,172,.3), rgba(140,153,172,0)),
    -moz-linear-gradient(
      #fff 15%, #e9ecf1 15%, #d2d9e1 50%, #bdc6d2 50%, #dfe7ed
    );
  background-size:20px 10px;
  box-shadow:0 1px 0 rgba(255,255,255,.9);
  -webkit-animation:m .6s linear infinite;
  -moz-animation:m .6s linear infinite;
}
::-webkit-progress-bar {
  display:none;
}
::-moz-progress-bar {
  visibility:hidden;
}
@-moz-document url-prefix(http://) {
  progress {width:60px; height:10px;}
}
{% endcodeblock %}

Via [Benjamin De Cock](deaxon.com)