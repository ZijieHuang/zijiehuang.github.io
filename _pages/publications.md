---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

Here you can find a list of my academic publications.  {% if site.author.googlescholar %} You can also find a list of my publications on <a href="{{site.author.googlescholar}}" style="color:#52adc8;">my Google Scholar profile</a> or via <a href="{{site.author.orcid}}" style="color:#52adc8;">my ORCID</a>. {% endif %} 

{% include base_path %}




<h2> Journal Articles </h2>


{% for post in site.publications reversed %}
  {% if post.published == 'journal' %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}



<h2> Conference Papers </h2>


{% for post in site.publications reversed %}
  {% if post.published == 'conference' %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}


<h2> Books </h2>



{% for post in site.publications reversed %}
  {% if post.published == 'books' %}
     {% include archive-single.html %}
  {% endif %}
{% endfor %}