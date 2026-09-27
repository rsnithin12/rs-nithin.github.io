---
show: true
width: 8
date: 2022-01-12 00:01:00 +0800
---

<!-- Scholarships -->
<div class="p-4">
    <h5>Scholarships</h5>
    <hr />
    <ul class="list-unstyled mb-1">
        {% for item in site.data.profile.scholarships %}
        <li class="media mb-2">
            {% if item.logo %}
            <img
                src="{{ item.logo | relative_url }}"
                alt="{{ item.name }}"
                style="width: 58px;"
                class="mr-2 mt-1">
            {% endif %}
            <div class="media-body">
                <div>
                    <strong>{{ item.name }}</strong>
                </div>
                <div class="small d-flex">
                    {% if item.institute %}
                    <div>
                        <strong>{{ item.institute }}</strong>
                    </div>
                    {% endif %}
                    {% if item.date %}
                    <div class="ml-auto no-break">
                        <em><strong>{{ item.date }}</strong></em>
                    </div>
                    {% endif %}
                </div>
                {% if item.infoscholarship %}
                <div class="small text-muted">
                    {{ item.infoscholarship }}
                </div>
                {% endif %}
            </div>
        </li>
        {% endfor %}
    </ul>
</div>
