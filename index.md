---
layout: default
title: "Home"
---

<div class="home-intro">
  <h1>Zo-Dns</h1>
  <p>Notes on Reverse Engineering, Malware Analysis, and Security.</p>
  <hr style="border: 0; border-top: 1px solid #e8e8e8; margin: 20px 0;">
</div>

### Recent Posts

<ul style="list-style: none; padding-left: 0;">
{% for post in site.posts %}
  <li style="margin-bottom: 12px; display: flex; justify-content: space-between; align-items: baseline;">
    <a href="{{ post.url | relative_url }}" style="font-weight: 500; text-decoration: none;">
      {{ post.title }}
    </a>
    <span style="color: #828282; font-size: 0.9em; font-family: monospace;">
      {{ post.date | date: "%Y-%m-%d" }}
    </span>
  </li>
{% endfor %}
</ul>
