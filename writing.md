---
layout: default
permalink: /writing.html
---

<section id="writing">
    <h2>Writing</h2>
    <ul id="blog-posts">
        {% for post in site.posts %}
        <li>
            <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
            <span class="date">{{ post.date | date: "%B %d, %Y" }}</span>
        </li>
        {% endfor %}
    </ul>
</section>

