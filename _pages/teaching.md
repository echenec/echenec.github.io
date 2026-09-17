---
layout: page
permalink: /teaching/
title: teaching
description: ""
nav: true
nav_order: 3
calendar: false
---


<style>
.teaching-category { font-size: 1.4em; font-weight: 700; border-bottom: 1px solid currentColor; padding-bottom: 0.3em; margin-top: 2em; margin-bottom: 0.5em; }
.teaching-statement { margin-bottom: 2em; }
.course-name { text-transform: uppercase; font-weight: 800; letter-spacing: 0.03em; font-size: 0.95em; margin-top: 1.2em; margin-bottom: 0.1em; }
.course-sems { font-weight: 400; font-size: 0.85em; margin-bottom: 0.4em; }
.course-inst { font-weight: 400; font-size: 0.85em; margin-bottom: 0.4em; }
.course-description { margin-bottom: 0.4em; }
.course-materials { font-size: 0.8em; }
.course-materials a { color: var(--global-theme-color, #2262c6); text-decoration: underline; }
.course-entry { margin-bottom: 1.8em; }
</style>

<p class="teaching-statement">
Under construction...
</p>

{% assign ta_courses = site.data.teaching | where: "role", "ta" %}
{% assign other_courses = site.data.teaching | where: "role", "other" %}

<div class="teaching-category">Teaching Assistant</div>
{% for c in ta_courses %}
<div class="course-entry">
<div class="course-name">{{ c.course }}</div>
<div class="course-sems">{{ c.sems }}</div>
<div class="course-inst">{{ c.inst }}</div>
<div class="course-description">{{ c.description }}</div>
{% if c.materials %}
<div class="course-materials">
{% for m in c.materials %}{% unless forloop.first %} &middot; {% endunless %}<a href="{{ m.url }}" target="_blank">{{ m.label }}</a>{% endfor %}
</div>
{% endif %}
</div>
{% endfor %}


<div class="teaching-category">Anonymous Teaching Evaluations</div>
<p>
  <i>Eva is great! In her discussion sections, there was a good balance between her speaking, asking questions, and our responding and facilitating the discussion</i> (The Social World, Spring 2026)
</p>

<p>
  <i>I really enjoyed having Eva as a TA. I think we won the jackpot. She was very kind, thorough, competent, and fair. </i> (Methods for Social Research, Fall 2025)
</p>

<p>
  <i>Eva Chen is an outstanding TA. She answers all questions clearly and thoroughly, and her approachable demeanor makes it easy to seek help or clarification. She’s incredibly quick and efficient, ensuring that no time is wasted, and her sessions are always well-planned, engaging, and incredibly useful. Honestly, her discussion sections were the best part of this course—they added so much value and made the material far more accessible and enjoyable. </i> (Methods for Social Research, Fall 2024)
</p>

<p>
  <i>Such an incredible TA! She worked to connect really difficult theory texts to contemporary ideas, as well as simplfied them and explained them really well. She was so understanding too, and so respectful of her students. i also loved the structure of the class, in which a broad question was posed, we would discuss it in groups, and then return to the larger class. This allowed for truly facinating conversations and helped me understand and contexualize the course material well.</i> (Social Theory, Spring 2024)
</p>

<p>
  <i>Eva is a very friendly and personable teacher in my opinion, as I always felt like I could go to her with questions if I ever had them or issues in my personal life that may bar my ability to come to class or turn in assignments on time. Additionally, I feel that she was able to communicate the readings on our syllabus in a very effective manner with the limited time we had each week, and I came out of each discussion section feeling like my understanding of the readings had received a proper bow to tie it all together.</i> (Social Theory, Spring 2024)
</p>

<p>
  <i>Eva was a great discussion leader! She really helped clarify concepts from lecture and it felt easy to participate in discussion because of the environment she created </i>(The Social World, Fall 2023)
</p>


