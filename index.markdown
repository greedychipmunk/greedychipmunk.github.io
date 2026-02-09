---
layout: default
title: Home
---

## Welcome! 👋

Thanks for stopping by. This is my personal space for learning, experimenting, and sharing what I discover along the way.

### 📚 What You'll Find Here

<div style="margin: 2rem 0;">
  <div style="margin-bottom: 1.5rem;">
    <h4 style="margin-bottom: 0.5rem;">
      <a href="/fiftytwolearn">🎯 Fifty Two Learn</a>
    </h4>
    <p style="margin-left: 1rem; color: #666;">
      My 2026 learning journey - tracking 52 weeks of new skills, technologies, and certifications
    </p>
  </div>

  <div style="margin-bottom: 1.5rem;">
    <h4 style="margin-bottom: 0.5rem;">
      <a href="/resume">💼 Resume</a>
    </h4>
    <p style="margin-left: 1rem; color: #666;">
      Professional experience and technical skills
    </p>
  </div>

  <div style="margin-bottom: 1.5rem;">
    <h4 style="margin-bottom: 0.5rem;">
      <a href="/prompts/">💡 Prompts</a>
    </h4>
    <p style="margin-left: 1rem; color: #666;">
      Collection of useful and effective AI prompts and ideas
    </p>
  </div>

  <div style="margin-bottom: 1.5rem;">
    <h4 style="margin-bottom: 0.5rem;">
      <a href="/about/">ℹ️ About</a>
    </h4>
    <p style="margin-left: 1rem; color: #666;">
      Learn more about this site
    </p>
  </div>
</div>

### 📝 Recent Posts

{% for post in site.posts limit:5 %}
  <div style="margin: 1rem 0; padding: 0.5rem 0; border-bottom: 1px solid #eee;">
    <a href="{{ post.url | relative_url }}" style="font-weight: 500;">{{ post.title }}</a>
    <br>
    <small style="color: #999;">{{ post.date | date: "%B %-d, %Y" }}</small>
  </div>
{% endfor %}

---

*Part laboratory, part confessional. These are my attempts to turn trial and error into something resembling expertise.*
