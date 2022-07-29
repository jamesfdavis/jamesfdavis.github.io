---
layout: default
title: "Software Engineer Solopreneur"
---

{% for post in site.posts %}

{: .text-black .text-lg .font-semibold .px-2}
[{{post.title}}]({{ post.url }}){:class="hover:text-gray-600 hover:underline"}

{: .font-mono .text-xs .py-1 .px-2 .uppercase .font-semibold .text-gray-500}
{{ post.date | date: "%d %B, %Y" }}

{: .pb-6 .px-2}
{{post.excerpt}}

{% endfor %}
