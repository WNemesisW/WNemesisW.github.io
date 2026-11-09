---
permalink: /
title: "Cyber situation awareness in research and practice"
excerpt: "Jouni Ihanus – PhD candidate and cyber security practitioner working on cyber situation awareness and deception technologies."
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a PhD candidate in cyber security at the University of Jyväskylä and a practitioner with almost twenty years in networks and cyber defence – first building networks, then leading the teams that make sense of what happens in them. One question runs through both my research and my practice: why is it so difficult to turn the data we already have into genuine understanding?

## Research
My doctoral research examines how deception technologies – honeypots, honeytokens and other low-false-positive sensors – can be integrated into cyber defence ecosystems as structured sources of cyber situation awareness. Following the Design Science Research paradigm, I develop and evaluate models and implementation concepts for security operations. The dissertation is expected to be completed in 2027. → [Publications](/publications/)

## Work
I am Chief Operating Officer at NGIT Oy. Previously I led Finnair's Cyber Defense Center, where I built the operating model for near real-time situational awareness in a safety-critical global airline. At Kela's Technical Situation Awareness Centre I led the group responsible for daily security operations and the situation awareness and response capability across the organisation. → [CV](/cv/)

## Exercises and teaching
Cyber exercises offer a controlled setting for studying decision-making under pressure. I have taken part in Locked Shields four times, leading the situation awareness team when Finland won in 2022, and I am co-organiser and scenario lead of ERIK, the largest annual cyber exercise of the National Defence Training Association of Finland (MPK). At Savonia University of Applied Sciences I teach communication and influence in comprehensive security at master's level.

## Current interests
I am particularly interested in how AI can support the analysis of security data so that it becomes useful for decision-making. In a self-built lab environment I am validating deception technologies and AI-assisted alert triage.

## Latest

<ul>
{% for post in site.posts limit:1 %}  <li>Blog: <a href="{{ post.url | relative_url }}">{{ post.title }}</a> ({{ post.date | date: "%B %Y" }})</li>
{% endfor %}{% assign latest_pubs = site.publications | sort: "date" | reverse %}{% for pub in latest_pubs limit:2 %}  <li>Publication: <a href="{{ pub.url | relative_url }}">{{ pub.title }}</a> ({{ pub.date | date: "%Y" }})</li>
{% endfor %}</ul>
