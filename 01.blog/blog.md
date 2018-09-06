---
title: Blog
blog_url: blog
menu: Blog

sitemap:
    changefreq: monthly
    priority: 1.03

content:
    items: @self.children
    order:
        by: date
        dir: desc
    limit: 5
    pagination: true

feed:
    description: 'The books I read, the food I make, and the games I play'
    limit: 25

pagination: true
---

# My Blog
