---
layout: about
title: about
permalink: /
subtitle: <a href='#'>Affiliations</a>. Address. Contacts. Motto. Etc.

profile:
  align: right
  image: prof_pic.jpg
  image_circular: true # crops the image to make it circular

selected_papers: false # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page

announcements:
  enabled: false # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: false
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---

Hi, I'm Lennart Weissenstein, a Unity Developer and Technical Artist based in Berlin. I enjoy creating interactive experiences, from 3D environments to smaller-scale games and prototypes.  

I'm currently studying International Media Informatics at HTW Berlin, focusing on Game Design, 3D Modeling, and Materials/Asset Optimization. I have experience working on collaborative team projects both at university and professionally, including co-creating a serious game prototype with Food4Future and IGZ, as well as completing solo projects such as 3D models and a 2D endless shooter game.  

I am focused on further developing my skills as a Game Designer, 3D Artist, and Technical Artist, contributing to projects where creativity and technical precision are valued.  

Connect with me on [LinkedIn](https://www.linkedin.com/in/lennart-weissenstein/) and check out my work on [GitHub](https://github.com/lweissenstein).

<div class="projects">
  <h2 class="category">selected projects</h2>
  <div class="row row-cols-1 row-cols-md-3">
    {% assign all_projects = site.projects %}

    {% assign featured_projects = all_projects | where: "selected", true %}

    {% assign sorted_featured = featured_projects | sort: "importance" %}

    {% for project in sorted_featured %}
      {% include projects.liquid %}
    {% endfor %}

  </div>
</div>

Check out [all my projects](/projects/).