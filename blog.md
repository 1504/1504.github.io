---
layout: page
title: 
permalink: /blog/
---
<div class="mw7 center pb2">

  <div class="post-list">
    {% for post in site.posts %}
      <div>
      <h2>
          <a class="link black-80 underline dim" href="{{ post.url | prepend: site.baseurl }}">{{ post.title | escape }}</a>
        </h2>
        
        <span class="f4 black-50 i center">{{ post.date | date: "%b %-d, %Y" }}</span>
      </div>
    {% endfor %}
  </div>

</div>