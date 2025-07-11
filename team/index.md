---
title: Team
nav:
  order: 3
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %}Team

Do we want some other text here? So far:
We are **always** looking for new DPhil/MSc students and Postdocs to join the team [(see recruitment)]({{ site.url }}{{ site.baseurl }}/recruitment) **!**

{% include section.html %}

{% include list.html data="members" component="portrait" filter="role == 'pi'" %}
{% include list.html data="members" component="portrait" filter="role != 'pi'" %}

{% include section.html background="images/background.png" dark=true %}

Do we need this section? what would we put there? the marine ecology lab does not have it here.

{% include section.html %}

{% capture content %}

{% include figure.html image="images/group/group2024.JPG" %}

{% endcapture %}

{% include grid.html style="square" content=content %}
