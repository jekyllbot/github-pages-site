---
layout: default
title: GitHub Pages Example
---

TOC:
{:toc}

# GitHub Pages Example

## Build infos

<ul>
  <li><strong>Build time:</strong> {{ site.time | date_to_rfc822 }}</li>
  <li><strong>Unix build time:</strong> {{ site.time | date:"%s" }}</li>
  <li><strong>Jekyll version:</strong> {{ jekyll.version }</li>
</ul>

<h2 id="plugins">Plugins</h2>

<ul>
  <li>Hi @jekyllbot, this site is :sparkles:!</li>
  <li><a href="sitemap.xml">sitemap</a></li>
  <li><a href="feed.xml">feed</a></li>
</ul>

{% highlight ruby %}
def hi
  puts "Hello."
end
{% endhighlight %}

```ruby
def hi
  puts "Hello."
end
```

<h2 id="github-namespace">GitHub Namespace</h2>

<div id="output">&nbsp;</div>

<p><em>Pro-tip: The entire Jekyll <code>site</code> object is available via Javascript console.</em></p>

<script type="text/javascript" src="assets/renderjson.js"></script>
<script>var site = {"github": {{ site.github | jsonify }}};</script>
<script src="assets/behaviour.js"></script>
