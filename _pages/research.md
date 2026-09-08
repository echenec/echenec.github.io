---
layout: page
permalink: /research/
title: research
description: ""
nav: true
nav_order: 2
---

<style>
/* Research category */
.research-category {
  font-size: 1.4em;
  font-weight: 700;
  border-bottom: 1px solid currentColor;
  padding-bottom: 0.3em;
  margin-top: 2em;
  margin-bottom: 0.75em;
}

/* Short description */
.research-description {
  margin-bottom: 1.5em;
}

/* Subcategory */
.research-subcategory {
  font-size: 0.9em;
  font-weight: 400;
  letter-spacing: 0.04em;
  text-transform: uppercase;
  margin-top: 1.5em;
  margin-bottom: 0.75em;
}

/* Individual publication */
.research-publication {
  margin-bottom: 1.5em;
}

/* Smaller links */
.research-links {
  font-size: 0.8em;
}

.research-links a {
  color: var(--global-theme-color, #2262c6);
}

/* Remove bibliography numbering */
.bibliography {
  list-style: none;
  padding-left: 0;
}

.bibliography li {
  list-style: none;
}
</style>


<div class="research-category">Migration</div>

<div class="research-description">
Under construction...
</div>

<div class="research-subcategory">Under Review</div>

{% bibliography --query @*[keywords ~= migration && status = "Under review"] %}


<div class="research-subcategory">Work in Progress</div>

{% bibliography --query @*[keywords ~= migration && status = "Work in progress"] %}



<div class="research-category">Race &amp; Ethnicity</div>

<div class="research-description">
Under construction...
</div>


<div class="research-subcategory">Work in Progress</div>

{% bibliography --query @*[keywords ~= race-ethnicity && status = "Work in progress"] %}



<div class="research-category">Asian America</div>

<div class="research-description">
Under construction...
</div>


<div class="research-subcategory">Reviews</div>

{% bibliography --query @*[keywords ~= asian-america AND status = "Reviews"] %}
