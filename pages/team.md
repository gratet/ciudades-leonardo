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
    image_fullwidth: headers/platja_4.JPG
    background-color: "#262930"
    caption: Cambrils beach, Costa Daurada (Lluís Rovira Barenys/ revistacambrils.cat)
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
<img src="{{ site.urlimg }}team/{{ member.pic }}" alt="{{ member.name }}" style="padding:10px; border-radius: 50%;">
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

##### **_Alejandro González Domingo_**

***Precarious Livelihoods in the Making of a Tourist City: The Social Geography of Tourism Workers in Barcelona***

*Director: Dr. Antonio Russo*

This PhD thesis is developed within the framework of the H2020-SMARTDEST project. It aims to analyse how social precarity in the tourist city of Barcelona is produced, what consequences it has on workers' labour and residential trajectories, and what forms of coping emerge from different social positions to build spaces of solidarity and resilience. Through biographic interviews and panel data, I analyse the modes of existence affected by social precarization, the socio-spatial processes inherited to a tourist city and the relational agency of formal and informal tourism workers, during the period 2008 until the COVID-19 crisis. The principles of life course theory are implemented to understand with life transitions and key events that influence workers’ lives paths. Through this research I expect to contribute to reveal the specific social inequalities of the tourist city from an analysis of labour and social geography, the imbrications with tourist mobility regimes and forms of capitalism extractivism that influence over workers’ lives.

##### **_Maria Esperanza Medina Chavarria_**

***Reconfiguration of Visitor Flows and their Management in Natural Protected Areas since the Pandemic***

*Directors: Dr. Òscar Saladié Borraz and Dr. Aaron Gutiérrez Palomero.*

Natural protected areas (NPAs) are areas actively managed to accomplish purposes ranging from the conservation of natural values and services, the improvement of physical and mental well-being and the recreation of those who visit them. These sensitive areas can be negatively affected by contexts of rapid socio-economic and environmental transformations, such as the ones caused by the COVID-19 pandemic. In Spain, for instance, an increasing interest in NPAs was observed and proximity tourism resurfaced. This even meant that in certain periods, some NPAs were even more visited than before the pandemic, increasing the constraints and the risks associated to a greater anthropogenic activity. This research aims to understand the emerging challenges for the agents involved in the management of visitors in NPAs, as well as to identify the practical foundations that explain how and why they responded to these challenges the way they did. By retrieving information from academic production, digital media, and from the managers themselves, the effects of COVID-19 on tourist flows to NPAs, the application and adaptations of visitor management policies implemented in NPAs of Catalonia, and specifically, in the province of Tarragona, are being analyzed. An essential part of this research is the analysis of visitor behavior on a case study; that is, to comprehend the changes in the profile of current users of a Natural Park of Tarragona. The results will be relevant to understand their motivation and behavior in space and time. This information is key for the development of tools and strategies for a proper and efficient planning, management, monitoring, and evaluation system.

##### **_Ana Pastor Alcaraz_**

***Smartering governance: Power and agency in evolving destinations ecosystems.***

*Director: Dr. Antonio Russo*

This doctoral project’s main ambition is to explore relationships of power among the agents framed in a destination ecosystem, understood (and mapped) from a holistic perspective that involves both traditional and non-traditional tourism stakeholders, and how does that play out concerning the emergence of the “smart” paradigm as a sociotechnical regime which structures and reorders such power relations within governance structures and agendas at destination level. This is an area of enquiry in which consistent insights from the literature are relatively scarce. The rising relevance of non-traditional stakeholders and their agenda-setting power is also discussed through an examination of positionings and discourses on tourism development. Focusing on Barcelona as a case study on a temporal line stretching from the pre-covid to the post-pandemic period, this work questions concepts of destination resilience from an evolutionary perspective. Barcelona is presented in a context of evolving challenges, from the smart city neoliberal approach, the “overtourism” crisis, and post-pandemic tourism recovery and their implication in Barcelona's Economic Development Model, which focuses on technology sovereignty.

##### **_Oriol Gallardo Prat_**

***Smart Destinations and the enhancement of local tourism destinations’ local adaptability and resilience towards global challenges***

*Directors: Dr. Salvador Anton Clavé and Dr. Aaron Gutiérrez Palomero*

The current global change dynamics generate new economic, social and environmental challenges to tourism destinations. Within this context, local responses are needed to face new multiple growing vulnerabilities. Tourism destinations, understood as complex systems, must generate conditions that allow them to enhance their adaptative capacity and their resilience against these global challenges. Meanwhile, tourism destinations are in process of increasing integration of smart solutions in their planning and management, in the context of the so-called Smart Destinations. The objective of this PhD thesis will be to understand the contribution of Smart Destinations’ operative development in enhancing the destinations’ adaptative capacity and resilience towards the emerging global challenges.

##### **_Natalia Restrepo Montoya (defended on 2021-12-21)_**

[***El papel de las Instituciones en el Desarrollo Regional del Turismo: Una perspectiva desde la Densidad Institucional***](http://hdl.handle.net/10803/673175)

*Director: Dr. Salvador Anton Clavé.*

The aim of this thesis is to understand the role of institutions in regional tourism development. It analyses whether the generation of institutional capacities is a facilitator of the consolidation and tourist development processes of a region and a governance driver. For this purpose, the research deploys an analytic model inspired, in the context of the economic geography, in the institutional thickness approach, paying particular attention to the study of the role of institutional presence, the interaction dynamics, domain structures and the common agendas between institutions in tourist and regional development. The empirical analysis is developed in a Latin American region, Antioquia – Colombia. The research methodology combines qualitative and quantitative techniques applied directly to 28 key institutions for tourist development in the Antioquia region and in Colombia. There are another additionally analysed 79 institutions intervening indirectly which are associated to the tourist activity.

##### **_Maria Eugenia Altamirano (defended on 2023-03-17)_**

[***Placing favelas on the tourist city map: Between commodification and representation.***](https://www.tdx.cat/handle/10803/688205#page=1)

*Director: Dr. Antonio Russo.*

This doctoral thesis aims to analyse the role of tourism practices and performances as a socio-economic activity and its capacity, real and potential, to re-signify and transform the physical, social and cultural landscape of urban tourist destinations. The case study is based on informal urban settlements of Rio de Janeiro, locally known as favelas, which carry almost 30 years of controversial tourist development. The focus will be turned into the actor-networks created around certain slum tourism practices and performances to analyse whether there is or not a reconceptualisation of slums as legitimate urban agents although at the margins of the neo-liberal agenda. The outcome of this thesis draws on the part that the embodied interactions between tourism actors play on the process of tourist placemaking in its physical and symbolic level, as well as the negotiation of urban identities.

##### **_Alba Viana Lora (defended on 2023-10-16)_**

[***Impacto social de la investigación en turismo. Proyectos de planificación turística.***](http://hdl.handle.net/10803/689276))

*Director: Dra. Marta Nel-lo Andreu*

This thesis aims to deepen the analysis of the social impact of scientific research in tourism, as well as to explore the instruments available to evaluate and enhance it. The research carried out has culminated in five scientific articles, subjected to a rigorous peer review process and published in journals indexed in recognized impact indexes. Through this body of work, the aim is to address and provide answers to the five research questions posed. In the context of this study, the desire to contribute significantly to scientific knowledge, both theoretical and methodological, regarding the social impact of scientific research, with emphasis on the field of tourism, is based on this study. In order to carry out this work, a thorough analysis of evaluation methods has been undertaken, with the objective of designing a tool that identifies, measures and objectively visualizes the benefits that research provides to society, once the research has been published, disseminated and applied in the field of tourism. This research also delves into the identification of possible ways to enhance this social impact. Thus, it seeks to take research beyond the academic context, turning it into an effective tool to contribute value to society in general. Finally, this thesis should serve to highlight the need for greater awareness among researchers of the potential social impact of their work. This awareness not only has implications for the researcher him/herself, but also for the scientific community as a whole and for the society it serves. It encourages researchers to adopt a more proactive and reflective approach, considering the scope of their research beyond traditional academic spheres.

##### **_Alba Font Barnet (defended on 2023-11-2023)_**

***Multidimensional assessment to enhance the well-being benefits provided by nature areas. A participatory approach applied in different cases of Europe and Latin America.***

*Director: Dr. Marta Nel-lo Andreu*

Nature offers a wide range of health and well-being benefits, closely linked to the objective of providing genuine experiences that intend to involve visitors across the physical, mental, social, emotional, spiritual, and environmental dimensions. In this sense, tourism offering well-being practices in nature has increased exponentially in recent years, and the scientific interest has also grown at a similar rate, from both a theoretical and a methodological perspective.
This doctoral thesis follows the theoretical principle that natural protected areas can contribute to the sustainable development, and from the focus of how we manage parks, it gives us the opportunity to improve the health of both our nature and communities. The aim is to discern the potential opportunities of nature areas to provide well-being benefits to locals and tourists from management and public use. To provide scientific evidence and transfer knowledge on this topic, a mixed methodology is applied in different natural areas in Europe and Latin America. This research is applied within the framework of a methodological participatory process and co-creation approach that integrates visual methods in data collection and analysis, together with the involvement of public and private agents, locals, and tourists.
