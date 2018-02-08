### here be my collection of knowledge.
This automatic page generator is the easiest way to create beautiful pages for all of your projects. Author your page content here using GitHub Flavored Markdown, select a template crafted by a designer, and publish. After your page is generated, you can check out the new branch:

```
$ cd your_repo_root/repo_name
$ git fetch origin
$ git checkout gh-pages
$ git status
$ git diff
$ git add .
$ git commit -m "yippie"
$ git push
```

### Posts
---
layout: default
title: entries
---

{% for post in site.posts %}
### [{{ post.title }}]({{ post.url }}) {{ post.date | date: "%Y-%m-%d"}} | {{ post.content | number_of_words }} words

{{ post.excerpt | strip_html | truncatewords: 50 }}

{% endfor %}

### Authors and Contributors
You can @mention a GitHub username to generate a link to their profile. The resulting `<a>` element will link to the contributor's GitHub Profile. For example: In 2007, Chris Wanstrath (@defunkt), PJ Hyett (@pjhyett), and Tom Preston-Werner (@mojombo) founded GitHub.

### Support or Contact
Having trouble with Pages? Check out the documentation at http://help.github.com/pages or contact support@github.com and we’ll help you sort it out.
