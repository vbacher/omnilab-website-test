---
title: Team
nav:
  order: 1
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %}Team

Do we want some other text here?

The other group links to their lab handbook. We could do the same

So far:

We are **always** looking for new DPhil/MSc students and Postdocs to join the team [(see recruitment)]({{ site.url }}{{ site.baseurl }}/recruitment) **!**

{% include section.html %}

{% include list.html data="members" component="portrait" filter="group != 'alumni'" %}

{% include section.html background="images/misc/background.png" dark=true %}

Do we need this section? what would we put there? the marine ecology lab does not have it here.

{% include section.html %}

{% include figure.html image="images/group/group2024.JPG" width="100%" %}

## Alumni

{% include section.html %}

{% assign alumni_members = site.members | where: "group", "alumni" | sort: "left" | reverse %}
{% for member in alumni_members %}
{% include portrait.html
    name=member.name
    image=member.image
    role=member.role
    description=member.description
    left=member.left
    aliases=member.aliases
    links=member.links
    style="small"
  %}
{% endfor %}
