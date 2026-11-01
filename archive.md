---
layout: minimal
---
<style>
  body {
    font-family: "Times New Roman", Times, serif;
    line-height: 1.6;
    max-width: 800px;
    margin: 40px auto;
    padding: 0 20px;
  }
</style>

[← Back to Main Page](/)

---

# Jokes & Fun

This is the collection of my social media posts, thoughts, and writings from over the years.

<img src="assets/cover.png" alt="Page Cover" style="max-width: 100%; display: block; margin: 20px auto;">

## Hebrew (ניב מקומי)

<div dir="rtl" lang="he">
<ul>
  {% assign jokes = site.pages | where: "category", "joke" | sort: "date" | reverse %}
  {% for joke in jokes %}
    {% if joke.path contains "archive/he/" %}
      <li>
        <a href="{{ joke.url | relative_url }}">{{ joke.title }}</a>
        - {{ joke.date | date: "%d.%m.%Y" }}
      </li>
    {% endif %}
  {% endfor %}
</ul>
</div>

<hr style="width: 20%; border: 0; border-top: 1px solid #ccc; margin: 40px auto;">

## English (Nonlocal Dialect)

<ul>
  {% for joke in jokes %}
    {% if joke.path contains "archive/en/" %}
      <li>
        <a href="{{ joke.url | relative_url }}">{{ joke.title }}</a>
        - {{ joke.date | date: "%d.%m.%Y" }}
      </li>
    {% endif %}
  {% endfor %}
</ul>
