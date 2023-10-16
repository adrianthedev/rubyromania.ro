---
layout: default
title: "News"
---

<section class="container mx-auto py-8">
    <h1 class="text-3xl md:text-4xl font-bold mb-4">News</h1>

    <ul class="list-disc pl-6">
        {% for post in site.posts %}
        <li>
            <span class="text-blue-500">{{ post.date | date: "%B %-d, %Y" }}</span> &mdash; <a href="{{ post.url }}" class="hover:underline">{{ post.title }}</a>
        </li>
        {% endfor %}
    </ul>
</section>