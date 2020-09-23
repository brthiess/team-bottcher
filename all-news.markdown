---
layout: home
title: All News - Team Bottcher
permalink: /all-news/
---

{% include banner.html subpage="true" %}

<section class='media general-section'>
    <h2 class='text-header'>All News</h2>
    <div class='media-news-container'>
        {% for item in site.data.news %}
            <div class='news-item'>
                <a href="{{ item.link }}" class="news-link"></a>
                <div class='news-item-image-container'>
                    <img src='/assets/images/news/{{ item.image }}' alt="{{ item.subtitle }}"/>
                </div>
                <div class='news-item-subtitle'>{{item.subtitle}}</div>
                <div class='news-item-date'>{{item.date}}</div>
            </div>
            {% endfor %}
    </div>
</section>
