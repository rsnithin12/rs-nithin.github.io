---
show: true
width: 8
date: 2024-01-12 00:01:00 +0800
---

<!-- Honors and Awards -->
<div>
  <img
    data-src="{{ 'assets/images/covers/cover1.jpg' | relative_url }}"
    class="lazy w-100 rounded-xl"
    src="{{ '/assets/images/empty_300x200.png' | relative_url }}"
    style="height: 250px;">

  <div class="card-img-overlay"
       style="background: rgb(255,255,255,0.8); overflow-y: auto;">
    <h5 class="card-title">Honors &amp; Awards</h5>
    <ul class="list-unstyled mb-1">
      {% for item in site.data.profile.awards %}
      <li class="media mb-2">
        <img
          src="{{ item.logo | relative_url }}"
          alt="{{ item.name }}"
          style="width: 38px;"
          class="mr-1 mt-1">
        <div class="media-body">
          <div><strong>{{ item.name }}</strong></div>
          {% if item.institute %}
          <div class="small d-flex">
          <div><strong>{{ item.institute }}</strong></div>
          {% if item.date %}
            <div class="ml-auto no-break">
            <em><strong>{{ item.date }}</strong></em>
            </div>
          {% endif %}
          </div>
          {% endif %}
          <div class="small d-flex">
            {% if item.infoaward %}
            <div>
              {{ item.infoaward }}
            </div>
            {% endif %}
          </div>
        </div>
      </li>
      {% endfor %}
    </ul>
  </div>
</div>
