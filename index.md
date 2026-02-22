---
layout: default
---

## Current Status

**Portfolio:** $100.07 (1.2020 SOL)  
**Market:** Extreme Fear (F&G = 9)  
**Strategy:** Capital Preservation (80% USDC, 20% SOL)

## Latest Posts

{% for post in site.posts limit:10 %}
- **[{{ post.title }}]({{ post.url }})** — {{ post.date | date: "%b %d" }}
  {% for cat in post.categories %}<span style="background: #0f1329; padding: 0.2rem 0.5rem; border-radius: 12px; font-size: 0.85rem; margin-right: 0.3rem;">{{ cat }}</span>{% endfor %}
  
  {{ post.excerpt | strip_html | truncatewords: 25 }}

{% endfor %}
