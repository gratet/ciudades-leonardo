---
permalink: "/project/team/"
layout: page-fullwidth
title: "Who we are"
meta_title: "Who we are"
subheadline: "Meet the team"

teaser: "Some important info about the project Adaptour team." 

meta_teaser: "Metadata about..."


header:
    image_fullwidth: header_homepage_13.jpg
    background-color: "#262930"
    caption: 
---


Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.


<ul class="small-block-grid-2 medium-block-grid-3 large-block-grid-4">


{% for member in site.data.team %}


<li>
<div itemscope itemtype="http://schema.org/Person" style= "text-align: center;">

<h5>
{% if member.name %}
	{{ member.name }}<br>
{% endif %}

{% if member.lastname %}
	{{ member.lastname }}
{% endif %}
</h5>


{% if member.position %}
	{{ member.position }}<br/>
{% endif %}


<!-- click on image will navigate to the personal website -->
<!--<a class="th" href="{{ member.social.first.url }}">-->
<img src="{{ site.urlimg }}/team/{{ member.pic }}" alt="{{ member.name }}" style="padding:10px; border-radius: 50%;">
<!--</a>-->

<!-- social media icons -->
<ul class="inline-list" style="padding:10px">
	{% for email in member.email %}
              <li><a href="mailto:{{ email.url }}?subject=[ADAPTOUR] " class="{{ email.class }}" title="{{ email.title }}"></a></li>
	{% endfor %}


	{% for social in member.social %}
              <li><a href="{{ social.url }}" target="_blank" class="{{ social.class }}" title="{{ social.title }}"></a></li>
	{% endfor %}
</ul><!-- /.inline-list -->


{% if member.organization %}
	<strong>{{ member.organization }}</strong><br/>
{% endif %}

{% if member.department %}
	<i>{{ member.department }}</i><br/>
{% endif %}


<strong>Palabras clave:</strong>
<ul>
{% for keyword in member.keywords %}
	<li style="display:inline;"><code class="highlighter-rouge">{{ keyword }}</code></li>
{% endfor %}
</ul>



</div> <!-- http://schema.org/Person -->
</li>
{% endfor %}

