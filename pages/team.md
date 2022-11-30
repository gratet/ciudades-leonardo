---
permalink: "/team/"
layout: page-fullwidth
breadcrumb: true
title: "Who we are"
meta_title: "Who we are"
subheadline: "Meet the team"

teaser: "The ADAPTOUR project team is composed of 10 doctors in the Research Team and six doctors, seven doctoral students and one research assistant in the Working Team. The project will be coordinated by a senior and a junior Principal Investigator, both with experience in leading projects and a significant track of international research outputs. Members of the two teams belong to seven different research groups from five different research institutions which have previously collaborated. Fifty per cent of the whole team is composed of geographers (12) but it also includes researchers with background in political science (1), computer science (1), economics (2), sociology (2) and tourism studies (6)." 

meta_teaser: "Metadata about..."

header:
    image_fullwidth: headers/pers.JPG
    background-color: "#262930"
    caption: Aerial view of Cambrils, Costa Daurada (Lluís Rovira Barenys/ revistacambrils.cat)
---


<ul class="small-block-grid-1 medium-block-grid-2 large-block-grid-3">


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
<ul style="padding:10px;text-align: center;list-style-type: none">
	{% for email in member.email %}
              <li style="display: inline;padding:10px"><a href="mailto:{{ email.url }}?subject=[ADAPTOUR] " class="{{ email.class }}" title="{{ email.title }}"></a></li>
	{% endfor %}


	{% for social in member.social %}
              <li style="display: inline;padding:10px"><a href="{{ social.url }}" target="_blank" class="{{ social.class }}" title="{{ social.title }}"></a></li>
	{% endfor %}
</ul><!-- /.inline-list -->


{% if member.organization %}
	<strong>{{ member.organization }}</strong><br/>
{% endif %}

{% if member.department %}
	<i>{{ member.department }}</i><br/>
{% endif %}


<strong>Keywords:</strong>
<ul>
{% for keyword in member.keywords %}
	<li style="display:inline"><code class="highlighter-rouge">{{ keyword }}</code></li>
{% endfor %}
</ul>



</div> <!-- http://schema.org/Person -->
</li>
{% endfor %}

