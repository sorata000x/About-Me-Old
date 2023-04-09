---
layout: page
title: Projects
permalink: /projects/
---

{% for repo in site.github.public_repositories %}

{% if repo.name == 'Achievement' %}

## [{{ repo.name }}]({{ repo.html_url }})

{{ repo.description }}

Topics: {{ repo.topics | array_to_sentence_string }}

Last updated: {{ repo.updated_at | date_to_string }}

{% endif %}

{% if repo.name == 'Experience-Bar' %}

## [{{ repo.name }}]({{ repo.html_url }})

{{ repo.description }}

Topics: {{ repo.topics | array_to_sentence_string }}

Last updated: {{ repo.updated_at | date_to_string }}

{% endif %}

{% endfor %}
