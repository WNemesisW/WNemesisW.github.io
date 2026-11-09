---
permalink: /
title: "Cyber situation awareness in research and practice"
excerpt: "Jouni Ihanus – cyber security leader and doctoral researcher on cyber situation awareness and deception technologies."
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Hi, I'm Jouni. I've spent almost twenty years in networks and cyber defence – first building networks, then leading the teams that make sense of what happens in them. Along the way one question has stuck with me: why is it so hard to turn the data we already have into real understanding? It runs through both my work and my doctoral research.

## Research
At the University of Jyväskylä I study how deception technologies – honeypots, honeytokens and other low-false-positive sensors – can become structured building blocks of cyber situation awareness. I follow Design Science Research, so the goal is always something practical: models and implementation concepts a SOC can actually put to work. Dissertation expected in 2027. → [Publications](/publications/)

## Work
I'm COO at NGIT Oy. Before that I led Finnair's Cyber Defense Center, where I built the operating model for near real-time situational awareness in a safety-critical global airline. At Kela's Technical Situation Awareness Centre I led a 30-person group, two of its three teams working 24/7. → [CV](/cv/)

## Exercises and teaching
Cyber exercises are where theory meets pressure. I've taken part in Locked Shields four times and led the situation awareness team when Finland won in 2022. I'm also co-organiser and scenario lead of ERIK, the largest annual cyber exercise of the National Defence Training Association of Finland (MPK). At Savonia University of Applied Sciences I teach communication and influence in comprehensive security at master's level.

## Right now
I'm especially interested in how AI can turn security data into analysis that decision-makers can actually use. In my home lab I'm testing AI-assisted triage on top of deception data.

## Latest

<ul>
{% for post in site.posts limit:1 %}  <li>Blog: <a href="{{ post.url | relative_url }}">{{ post.title }}</a> ({{ post.date | date: "%B %Y" }})</li>
{% endfor %}{% assign latest_pubs = site.publications | sort: "date" | reverse %}{% for pub in latest_pubs limit:2 %}  <li>Publication: <a href="{{ pub.url | relative_url }}">{{ pub.title }}</a> ({{ pub.date | date: "%Y" }})</li>
{% endfor %}</ul>

## Get in touch
Always happy to talk about cyber situation awareness, exercise design or research collaboration: [Email](mailto:{{ site.author.email }}) · [LinkedIn](https://www.linkedin.com/in/{{ site.author.linkedin }})
