---
title: 'Thoughts on Cyber Exercises, Time Compression, and Situation Awareness'
date: 2026-05-02
permalink: /posts/2026/05/Thoughts_on_Cyber_Exercises/
redirect_from:
  - /posts/2026/03/Thoughts_on_Cyber_Exercises/
tags:
  - Situation Awareness
  - Cyber Exercise

# Texts of the figures (rendered by _includes/ih-flow.html and ih-strips.html)
figures:
  levels:
    lane_a: "Situation awareness (Endsley, 1995)"
    lane_b: "Under high time compression"
    caption: "Endsley’s three levels of situation awareness, and what happens to each of them under high time compression."
    steps:
      - label: "Level 1"
        title: "Perception"
        text: "of relevant elements"
        view: "May still function: data is visible."
      - label: "Level 2"
        title: "Comprehension"
        text: "of their meaning"
        view: "Collapses: meaning cannot be formed."
      - label: "Level 3"
        title: "Projection"
        text: "of future states"
        view: "Becomes nearly impossible."
  window:
    cells: 24
    heading: "Focus of attention: roughly 3–&#8288;5 chunks at a time (Cowan)"
    legend_window: "Time window a team considers"
    legend_event: "Event"
    unit: "in the window"
    axis: "Time →"
    caption: "A schematic illustration, not measured data: the same eight events at a real-world pace, under time compression, and after the team has reduced the size of the situation."
    rows:
      - label: "Real-world operations"
        events: [2, 5, 8, 11, 14, 17, 20, 23]
        window: [7, 18]
        note: "Events are spread out, and the window stays within the limit."
      - label: "Exercise with time compression"
        events: [9, 10, 11, 12, 13, 14, 15, 16]
        window: [7, 18]
        over: true
        note: "The same events arrive in less time, and the same window now exceeds the limit."
      - label: "How teams cope"
        events: [9, 10, 11, 12, 13, 14, 15, 16]
        window: [11, 14]
        note: "A narrower time window and a subset of signals fit again, but the rest of the situation is left out."
---
Throughout my career, I have had the opportunity to participate in a wide range of cyber exercises. Most recently, I took part in a large-scale multinational exercise. As a strong advocate of situation awareness, one design choice consistently stands out across these environments: **time compression**.

Within a limited exercise window, blue teams are exposed to a dense sequence of attacks, incidents, and coordination tasks — far more tightly packed than in real-world operations. The reason is practical: very few organizations can afford to run multi-week exercises. Compression is necessary.

# The Challenge

Time compression comes with a cost—especially when viewed through the lens of developing situation awareness. When time is compressed, two recurring challenges emerge:

- **Operational actions are not supported by a unified situation picture**  
  The cycles required to build a comprehensive situation picture are simply too slow, particularly when teams are dealing with multiple urgent issues simultaneously.

- **Operational awareness and reporting drift apart**  
  Decision-making and reporting become separate activities. They are often weakly connected — or even contradictory.

# Why Does This Happen?

A useful starting point is Mica Endsley’s model of situation awareness in dynamic systems, which I have referenced in several previous blogs. Endsley (1995) defines situation awareness as a three-level process:

1. Perception of relevant elements  
2. Comprehension of their meaning  
3. Projection of future states  

In cyber operations, we often assume that improving visibility (Level 1) will naturally lead to better understanding (Level 2). In reality, this transition is fragile — and highly sensitive to cognitive load.

This is where Nelson Cowan provides critical insight.

Cowan (2001) demonstrates that the human focus of attention is limited to roughly **3–5 meaningful units (“chunks”) at a time**. When the number of incoming stimuli exceeds this limit, the ability to process information meaningfully degrades rapidly. Time compression directly increases the rate of incoming stimuli, eventually leading to cognitive saturation.

**In Endsley’s terms:**
- Level 1 (perception) may still function — data is visible  
- Level 2 (comprehension) collapses — meaning cannot be formed  
- Level 3 (projection) becomes nearly impossible  

{% include ih-flow.html number=1 figure=page.figures.levels %}

**In Cowan’s terms:**
- The number of active elements exceeds the capacity of attention  
- The system cannot maintain a coherent internal representation  

Under high time compression, teams are forced — implicitly — to make a trade-off:

***Either act fast, or understand deeply — but not both at the same time.***

This is not a process failure. It is a cognitive constraint.

**To cope, teams naturally reduce complexity:**
- They narrow the time window they consider  
- They focus on a subset of signals  
- They ignore or postpone broader synthesis  

In effect, they reduce the size of the “situation” to something that fits within human cognitive limits.

{% include ih-strips.html number=2 figure=page.figures.window %}

# A Question for Exercise Design

First, it is important to remember that the goal of these exercises is not to avoid hitting a wall, but to understand how hard we will hit it. Pushing teams to their limits is intentional and necessary.

However, it would be interesting to explore whether reducing time compression by slightly extending the duration of exercises, could bring operational awareness and reporting closer together. Another option would be to introduce a more tightly integrated exercise track that explicitly incorporates strategic decision-making.

This could enable training for more prolonged, long-term conflict scenarios, rather than focusing solely on isolated critical incidents.

# References

- Endsley, M. R. (1995). *Toward a Theory of Situation Awareness in Dynamic Systems*. Human Factors.  

  https://doi.org/10.1518/001872095779049543

- Cowan, N. (2001). *The Magical Number 4 in Short-Term Memory: A Reconsideration of Mental Storage Capacity*. Behavioral and Brain Sciences.  

  https://doi.org/10.1017/S0140525X01003922