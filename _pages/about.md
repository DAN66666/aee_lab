---
title: 实验室简介
permalink: /about/
---

<p class="lab-kicker">{{ site.data.lab.subtitle }}</p>

{{ site.data.lab.about | markdownify }}

## 研究与实践

{% for direction in site.data.lab.directions %}
- **{{ direction.title }}**{% if direction.description != empty %}：{{ direction.description }}{% endif %}
{% endfor %}

[了解研究方向]({{ '/research/' | relative_url }}){: .btn .btn--primary}

## 交流与联系

{{ site.data.lab.recruitment }}

- **联系邮箱：** [{{ site.data.lab.email }}](mailto:{{ site.data.lab.email }})
- **实验室地址：** {{ site.data.lab.address }}
