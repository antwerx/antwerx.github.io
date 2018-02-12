### here be my collection of knowledge.
I hope to collect bits of knowledge I have scattered around in various tools.
```
$ git status
$ git diff
$ git add .
$ git commit -m "yippie"
$ git push
```
### Posts

{% for post in site.posts %}
### [{{ post.title }}]({{ post.url }}) {{ post.date | date: "%Y-%m-%d"}} | {{ post.content | number_of_words }} words

{{ post.excerpt | strip_html | truncatewords: 50 }}

{% endfor %}

### Authors and Contributors
You can @mention a GitHub username to generate a link to their profile. The resulting `<a>` element will link to the contributor's GitHub Profile.

### Support or Contact
Having trouble with Pages? Check out the documentation at http://help.github.com/pages or contact support@github.com and we’ll help you sort it out.
