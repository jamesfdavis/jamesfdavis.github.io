---
layout: default
title: "Software Engineering Blog"
---

{: .text-black .text-xl .font-semibold}
<!-- # Penrose Development -->

<!-- {% for tag in site.tags %}

  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %} -->

{% for post in site.posts %}

{: .text-black .text-lg .font-semibold}
[{{post.title}}]({{ post.url }}){:class="hover:text-gray-600 hover:underline"}

{: .font-mono .text-xs .py-1 .uppercase .font-semibold .text-gray-500}
{{ post.date | date: "%d %B, %Y" }}

{: .pb-6}
{{post.excerpt}}

{% endfor %}
