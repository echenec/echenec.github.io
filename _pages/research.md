---
layout: page
permalink: /research/
title: research
description: ""
nav: true
nav_order: 2
---

<style>
.research-category { font-size: 1.4em; font-weight: 700; border-bottom: 1px solid currentColor; padding-bottom: 0.3em; margin-top: 2em; margin-bottom: 0.5em; }
.research-description { font-weight: 400; margin-bottom: 1em; }
.pub-subcategory { text-transform: uppercase; font-weight: 800; letter-spacing: 0.03em; font-size: 0.95em; margin-top: 1.2em; margin-bottom: 0.1em; }
.pub-entry { font-size: 1em; margin-bottom: 0.4em; }
.pub-year { font-weight: 400; font-size: 0.85em; margin-bottom: 0.4em; }
.pub-journal { font-size: 1em; margin-bottom: 0.4em; font-style: italic; }
.pub-author-me { font-weight: 700; font-style: normal; }
.pub-links { font-size: 0.8em; }
.pub-links a { color: var(--global-theme-color, #2262c6); text-decoration: underline; }
</style>

{% assign status_order = "Peer-Reviewed Publications,Forthcoming,Under Review,Working Papers,Work in Progress,Reviews" | split: "," %}

{% assign migration_items = site.data.publications | where: "category", "migration" %}
{% assign race_items = site.data.publications | where: "category", "race-ethnicity" %}
{% assign asian_items = site.data.publications | where: "category", "asian-america" %}



<div class="research-category">Temporary Migration</div>
<p class="research-description">
  My dissertation research how migrants holding temporary legal status navigate uncertain futures in their long-term decision-making, as well as in daily life. How do migrants navigate tensions between their individual migration goals and external pressures that discourage permanent settlement? When time in the host country does not guarantee legal stability, what other factors may foster a sense of settledness for new arrivals in the United States?
</p>
{% for status in status_order %}
{% assign matches = migration_items | where: "status", status %}
{% if matches.size > 0 %}
<div class="pub-subcategory">{{ status }}</div>
{% for pub in matches %}
<div class="pub-entry">
<div class="pub-year">{{ pub.year }}</div>
{{ pub.title }}
{% if pub.journal %}<br><span class="pub-journal">{{ pub.journal }}</span>{% endif %}
<br>
{% for author in pub.authors %}{% if author.last == "Chen" and author.first == "Eva" %}<span class="pub-author-me">{{ author.first }} {{ author.last }}</span>{% else %}{{ author.first }} {{ author.last }}{% endif %}{% unless forloop.last %}{% if forloop.rindex == 2 %} and {% else %}, {% endif %}{% endunless %}{% endfor %}
{% if pub.doi or pub.pdf or pub.preregistration or pub.data or pub.equal_authorship %}
<div class="pub-links">
{% if pub.doi %}<a href="https://doi.org/{{ pub.doi }}" target="_blank" rel="noopener">paper</a>{% endif %}
{% if pub.pdf %} &middot; <a href="/assets/pdf/{{ pub.pdf }}" target="_blank">paper</a>{% endif %}
{% if pub.preregistration %} &middot; <a href="{{ pub.preregistration }}" target="_blank" rel="noopener">preregistration</a>{% endif %}
{% if pub.data %} &middot; <a href="{{ pub.data }}" target="_blank" rel="noopener">data</a>{% endif %}
{% if pub.equal_authorship %} &middot; Equal authorship{% endif %}
</div>
{% endif %}
</div>
{% endfor %}
{% endif %}
{% endfor %}



<div class="research-category">Racial Categorization</div>
<p class="research-description">
  This line of research considers how the meaning of racial and ethnic categories shifts across individuals and contexts. How do group boundaries shift when material outcomes are at stake? Across multiple dimensions of stratification and inequality, what characteristics determine who counts as an insider versus an outsider?
</p>
{% for status in status_order %}
{% assign matches = race_items | where: "status", status %}
{% if matches.size > 0 %}
<div class="pub-subcategory">{{ status }}</div>
{% for pub in matches %}
<div class="pub-entry">
<div class="pub-year">{{ pub.year }}</div>
{{ pub.title }}
{% if pub.journal %}<br><span class="pub-journal">{{ pub.journal }}</span>{% endif %}
<br>
{% for author in pub.authors %}{% if author.last == "Chen" and author.first == "Eva" %}<span class="pub-author-me">{{ author.first }} {{ author.last }}</span>{% else %}{{ author.first }} {{ author.last }}{% endif %}{% unless forloop.last %}{% if forloop.rindex == 2 %} and {% else %}, {% endif %}{% endunless %}{% endfor %}
{% if pub.doi or pub.pdf or pub.preregistration or pub.data or pub.equal_authorship %}
<div class="pub-links">
{% if pub.doi %}<a href="https://doi.org/{{ pub.doi }}" target="_blank" rel="noopener">paper</a>{% endif %}
{% if pub.pdf %} &middot; <a href="/assets/pdf/{{ pub.pdf }}" target="_blank">paper</a>{% endif %}
{% if pub.preregistration %} &middot; <a href="{{ pub.preregistration }}" target="_blank" rel="noopener">preregistration</a>{% endif %}
{% if pub.data %} &middot; <a href="{{ pub.data }}" target="_blank" rel="noopener">data</a>{% endif %}
{% if pub.equal_authorship %} &middot; Equal authorship{% endif %}
</div>
{% endif %}
</div>
{% endfor %}
{% endif %}
{% endfor %}



<div class="research-category">Asian America</div>
<p class="research-description">
  My research interest also extends into Asian American studies. I consider how unique migration histories, legacies of racism, and relationships to imperialism shape contemporary Asian American political participation and group solidarity. 
</p>
{% for status in status_order %}
{% assign matches = asian_items | where: "status", status %}
{% if matches.size > 0 %}
<div class="pub-subcategory">{{ status }}</div>
{% for pub in matches %}
<div class="pub-entry">
<div class="pub-year">{{ pub.year }}</div>
{{ pub.title }}
{% if pub.journal %}<br><span class="pub-journal">{{ pub.journal }}</span>{% endif %}
<br>
{% for author in pub.authors %}{% if author.last == "Chen" and author.first == "Eva" %}<span class="pub-author-me">{{ author.first }} {{ author.last }}</span>{% else %}{{ author.first }} {{ author.last }}{% endif %}{% unless forloop.last %}{% if forloop.rindex == 2 %} and {% else %}, {% endif %}{% endunless %}{% endfor %}
{% if pub.doi or pub.pdf or pub.preregistration or pub.data or pub.equal_authorship %}
<div class="pub-links">
{% if pub.doi %}<a href="https://doi.org/{{ pub.doi }}" target="_blank" rel="noopener">paper</a>{% endif %}
{% if pub.pdf %} &middot; <a href="/assets/pdf/{{ pub.pdf }}" target="_blank">paper</a>{% endif %}
{% if pub.preregistration %} &middot; <a href="{{ pub.preregistration }}" target="_blank" rel="noopener">preregistration</a>{% endif %}
{% if pub.data %} &middot; <a href="{{ pub.data }}" target="_blank" rel="noopener">data</a>{% endif %}
{% if pub.equal_authorship %} &middot; Equal authorship {% endif %}
</div>
{% endif %}
</div>
{% endfor %}
{% endif %}
{% endfor %}
