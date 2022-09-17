---
layout: page
title: Store
permalink: /store/
---

<ul class="post-list">
    {%- for post in site.categories.store -%}
    <li>
        <h3>
            <a class="post-link" href="{{ post.url | relative_url }}">
                <img src="{{post.splash_image}}"  alt=""/>
                <br />
                {{ post.title | escape }} &rarr;
            </a>
        </h3>
        {%- if site.show_excerpts -%}
            {{ post.excerpt }}
        {%- endif -%}
    </li>
    {%- endfor -%}
</ul>
