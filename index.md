---
layout: default
title: "Software Engineer Solopreneur"
---

{: .text-black .text-xl .font-semibold}

{% for post in site.posts %}

{: .text-black .text-lg .font-semibold}
[{{post.title}}]({{ post.url }}){:class="hover:text-gray-600 hover:underline"}

{: .font-mono .text-xs .py-1 .uppercase .font-semibold .text-gray-500}
{{ post.date | date: "%d %B, %Y" }}

{: .pb-6}
{{post.excerpt}}

{% endfor %}
