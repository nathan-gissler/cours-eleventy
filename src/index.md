---
title: Page principale
layout: "base.njk"
---

Ceci est la première page du site.

Voici tous les articles :

{% for article in collections.articles %}

- [{{ article.data.title }}]({{ article.url }})

{% endfor %}