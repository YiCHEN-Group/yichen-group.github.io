---
layout: default
title: Team
---

## Principal Investigator

{% for person in site.data.team %}
{% if person.position == "Principal Investigator" %}
<div class="team-card team-card--pi">
    {% if person.photo %}
    <img src="{{ person.photo }}" alt="{{ person.name }}" class="team-photo--pi">
    {% endif %}

    <div class="team-info">
        <h3 class="team-name">{{ person.name }}</h3>
        {% if person.email %}
        <p class="team-email">
            <a href="mailto:{{ person.email }}">{{ person.email }}</a>
        </p>
        {% endif %}
    </div>
</div>
{% endif %}
{% endfor %}

## PhD Students

<div class="team-grid">
{% for person in site.data.team %}
{% if person.position == "PhD Student" %}
<div class="team-card team-card--student">
    {% if person.photo %}
    <img src="{{ person.photo }}" alt="{{ person.name }}" class="team-photo--student">
    {% endif %}

    <div class="team-info">
        <h3 class="team-name">{{ person.name }}</h3>
        {% if person.year %}
        <p class="team-year">{{ person.year }}</p>
        {% endif %}
        {% if person.research %}
        <p class="team-research">{{ person.research }}</p>
        {% endif %}
        {% if person.email %}
        <p class="team-email">
            <a href="mailto:{{ person.email }}">{{ person.email }}</a>
        </p>
        {% endif %}
    </div>
</div>
{% endif %}
{% endfor %}
</div>

## Master Students

<div class="team-grid">
{% for person in site.data.team %}
{% if person.position == "Master Student" %}
<div class="team-card team-card--student">
    {% if person.photo %}
    <img src="{{ person.photo }}" alt="{{ person.name }}" class="team-photo--student">
    {% endif %}

    <div class="team-info">
        <h3 class="team-name">{{ person.name }}</h3>
        {% if person.year %}
        <p class="team-year">{{ person.year }}</p>
        {% endif %}
        {% if person.research %}
        <p class="team-research">{{ person.research }}</p>
        {% endif %}
        {% if person.email %}
        <p class="team-email">
            <a href="mailto:{{ person.email }}">{{ person.email }}</a>
        </p>
        {% endif %}
    </div>
</div>
{% endif %}
{% endfor %}
</div>

## Alumni

<div class="team-grid">
{% for person in site.data.team %}
{% if person.position == "Alumni" %}
<div class="team-card team-card--student">
    {% if person.photo %}
    <img src="{{ person.photo }}" alt="{{ person.name }}" class="team-photo--student">
    {% endif %}

    <div class="team-info">
        <h3 class="team-name">{{ person.name }}</h3>
        {% if person.year %}
        <p class="team-year">{{ person.year }}</p>
        {% endif %}
        {% if person.research %}
        <p class="team-research">{{ person.research }}</p>
        {% endif %}
        {% if person.email %}
        <p class="team-email">
            <a href="mailto:{{ person.email }}">{{ person.email }}</a>
        </p>
        {% endif %}
    </div>
</div>
{% endif %}
{% endfor %}
</div>
