---
title: Portfolio
banner: /img/banners/manhattan.jpg
---

<div class="big-list">
  <h1>Hacks and Demos</h1>
  <ul class="demos">
  {% for project in site.data.cv.software.hacks_and_demos %}
    <li class="demo">
      <a title="Link opens in new window" target="_blank" href="{{ project.url }}">
        <div class="image"><img src="{{ project.picture }}" /></div>
        <div class="name"><p>{{ project.name }}</p></div>
      </a>
    </li>
  {% endfor %}
  </ul>

  <h1>Software Projects</h1>
  <ul>
  {% for project in site.data.cv.software.personal_projects %}
    <li>
      <a title="Link opens in new window" target="_blank" href="{{ project.url }}">{{ project.name }}</a> {{ project.summary }}
    </li>
  {% endfor %}
  </ul>

  <h1>Open Source Contributions</h1>
  <ul>
  {% for project in site.data.cv.software.open_source_contributions %}
    <li>
      <a title="Link opens in new window" target="_blank" href="{{ project.url }}">{{ project.name }}</a> {{ project.summary }}
    </li>
  {% endfor %}
  </ul>

  <h1>Websites</h1>
  <ul>
  {% for project in site.data.cv.software.websites %}
    <li>
      <a title="Link opens in new window" target="_blank" href="{{ project.url }}">{{ project.name }}</a> {{ project.summary }}
    </li>
  {% endfor %}
  </ul>
</div> <!-- /.big-list -->
