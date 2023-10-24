---
layout: default
title: "News"
---

<section class="container mx-auto py-8">
    <h1 class="text-3xl md:text-4xl font-bold mb-4">News</h1>

    <ul class="divide-y divide-gray-300">
        {% for post in site.posts %}
        <li class="py-4">
            <a href="{{ post.url }}" class="text-blue-500 text-2xl font-semibold hover:underline">{{ post.title }}</a>
            <div class="text-gray-600">{{ post.date | date: "%B %-d, %Y" }}</div>
            <p class="mt-2">{{ post.excerpt | strip_html | truncate: 100 }}</p>
        </li>
        {% endfor %}
    </ul>
</section>