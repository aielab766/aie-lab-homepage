---
title: "AIE LAB - Team"
layout: gridlay
excerpt: "AIE LAB: Team members"
sitemap: false
permalink: /team/
---

# Team Members
At AIE LAB 766&423, students from various majors within the School of Information and Artificial Intelligence come together to collaborate and innovate. By 2024, the team had grown to nearly 20 outstanding members, with some continuing their studies at prestigious institutions such as USTC, UCAS, SEU, and NJU.

(Please click the name below for the lab memeber's profile)

---

## Mentor
{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if member.group == 0 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4><a href="{{ member.url }}" class="off">{{ member.name }}</a></h4>
  <i>{{ member.info }}</i>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

---
## Undergraduate Students
{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if member.group == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" 
     style="width: 115px; height: 115px; object-fit: cover; float: left; margin-right: 10px;" />
  <h4><a href="{{ member.url }}" class="off">{{ member.name }}</a></h4>
  <i>{{ member.info }}</i>

  <i>{{ member.description }}</i>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

---

## Alumni

{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if member.group == 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" 
     style="width: 115px; height: 115px; object-fit: cover; float: left; margin-right: 10px;" />
  <h4><a href="{{ member.url }}" class="off">{{ member.name }}</a></h4>
  <i>{{ member.info }}</i>

  <i>{{ member.description }}</i>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<!-- ---

## Administrative Support
Please contact our lab manager, <a href="mailto:Clif.Duhn@ucsf.edu">Clif Duhn</a>. -->









