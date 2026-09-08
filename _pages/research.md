---
layout: page
permalink: /research/
title: research
description: ""
nav: true
nav_order: 2
---

<style>
.research-category {
  font-size: 1.4em;
  font-weight: 700;
  border-bottom: 1px solid currentColor;
  padding-bottom: 0.3em;
  margin-bottom: 0.5em;
}

.research-description {
  font-weight: 400;
  margin-bottom: 1em;
}

.pub-entry {
  margin-bottom: 2em;
}

.pub-subcategory {
  font-weight: 600;
  margin-bottom: 0.3em;
}

.pub-links {
  font-size: 0.8em;
  margin-top: 0.35em;
}

.pub-links a {
  color: var(--global-theme-color, #2262c6);
  text-decoration: underline;
}
</style>

<details open>
<summary><strong>Migration</strong></summary>

<p class="research-description">
*Under construction*
</p>

{% bibliography --query @*[keywords ~= migration] %}

</details>

<details open>
<summary><strong>Race &amp; Ethnicity</strong></summary>

<p class="research-description">
*Under construction*
</p>

{% bibliography --query @*[keywords ~= race-ethnicity] %}

</details>

<details open>
<summary><strong>Asian America</strong></summary>

<p class="research-description">
*Under construction*
</p>

{% bibliography --query @*[keywords ~= asian-america] %}

</details>
