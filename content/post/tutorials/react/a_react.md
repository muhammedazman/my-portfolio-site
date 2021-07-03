---
title: "Hugo Tania Theme"
date: 2020-11-26
description: Make a blog with hugo tania theme!
draft: true
weight: 1
link: https://github.com/WingLim/hugo-tania
repo: https://github.com/WingLim/hugo-tania
icon: 📝
---

# Title

## Categorie 1

[TOC]

Hello, this is my first blog page. Firstly, i want to tell that we orden following page:

```html
<section>
    <h2>
        Latest Articles.
        <a class="section-button" href="/articles">View all</a>
    </h2>
    <div class="posts">
        {{ range $pages.Pages }}
        <div class="post">
            <a href="{{ .RelPermalink }}">
                <div class="post-row">
                    <time>{{ .Date.Format "Jan 02" }}</time>
                    <h3>{{ .Title }}</h3>
                </div>
                <!--<div class="new-post">New!</div>-->
            </a>
        </div>
        {{ end }}
    </div>
</section>
```