---
layout: page
permalink: /research/
title: research
description: ""
nav: true
nav_order: 2
---

<style>
/* Research category header */
.research-category {
  font-size: 1.4em;
  font-weight: 700;
  border-bottom: 1px solid currentColor;
  padding-bottom: 0.3em;
  margin-bottom: 0.5em;
  cursor: pointer;
}

/* Description */
.research-description {
  font-weight: 400;
  margin-bottom: 1em;
}

/* Type of work */
.pub-subcategory {
  text-transform: uppercase;
  font-weight: 300;
  letter-spacing: 0.03em;
  font-size: 0.85em;
  margin-bottom: 0.2em;
}

/* Publication title */
.pub-entry {
  font-weight: 400;
  margin-bottom: 1.5em;
}

.pub-year {
  font-weight: 700;
}

.pub-journal {
  font-style: italic;
}

.pub-author-me {
  font-weight: 700;
}

/* Links row */
.pub-links {
  font-size: 0.8em;
}

.pub-links a {
  color: var(--global-theme-color, #2262c6);
  text-decoration: underline;
}


  

<details open>
<summary><strong>Migration</strong></summary>

<p>
*Under construction*
</p>

{% bibliography --query @*[keywords ~= migration] %}

</details>


<details open>
<summary><strong>Race & Ethnicity</strong></summary>

<p>
*Under construction*
</p>

{% bibliography --query @*[keywords ~= race-ethnicity] %}

</details>


<details open>
<summary><strong>Asian America</strong></summary>
  
<p>
*Under construction*
</p>

{% bibliography --query @*[keywords ~= asian-america] %}


</details>
