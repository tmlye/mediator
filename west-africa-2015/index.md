---
layout: page
title: West Africa 2015
permalink: /west-africa-2015/
---
In January 2015 a friend and I drove from Nuremberg, Germany to Mali on our motorcycles. We spent some time in Morocco, before we headed further down through Mauretania, Senegal and on to Mali.
You can take a look at our [route]({{site.baseurl}}/west-africa-2015/route/) for more details.
The whole journey took a little over 4 months.
We travelled on two Honda Transalp, 23 and 17 years old.
If you're interested in what equipment we used, take a look at our [packing list]({{site.baseurl}}/west-africa-2015/packing-list).

Here are all posts that I wrote on this trip:

{% for post in site.categories.west-africa-2015 %}
  <article class="post" itemscope itemtype="https://schema.org/BlogPosting" role="article">
    <div class="article-item">
      <header class="post-header">
          <h2 class="post-title" itemprop="name"><a href="{{site.baseurl}}{{ post.url }}" itemprop="url">{{ post.title }}</a></h2>
      </header>
      <section class="post-excerpt" itemprop="description">
        <p>{{ post.content | strip_html | truncatewords: 50 }}</p>
      </section>
      <div class="post-meta">
        <time datetime="{{ post.date | date_to_long_string }}">{{ post.date | date_to_long_string }}</time>
      </div>
    </div>
  </article>
{% endfor %}
