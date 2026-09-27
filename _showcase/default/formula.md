---
show: true
width: 8
date: 2020-01-14 00:01:00 +0800
---

<!-- Positions -->
<div class="p-4">
    <h5>Positions &amp; Memberships</h5>
    <hr />
    <ul class="list-unstyled mb-1">
        {% for item in site.data.profile.memberships %}
        <li class="media mb-2">
            {% if item.logo %}
            <img
                src="{{ item.logo | relative_url }}"
                alt="{{ item.name }}"
                style="width: 38px;"
                class="mr-2 mt-1">
            {% endif %}
            <div class="media-body">
                <div>
                    <strong>{{ item.name }}</strong>
                </div>
                <div class="small d-flex">
                    {% if item.institute %}
                    <div>
                        {{ item.institute }}
                    </div>
                    {% endif %}
                    {% if item.date %}
                    <div class="ml-auto no-break">
                        <em>{{ item.date }}</em>
                    </div>
                    {% endif %}
                </div>
                {% if item.infoscholarship %}
                <div class="small text-muted">
                    {{ item.infoposition }}
                </div>
                {% endif %}
            </div>
        </li>
        {% endfor %}
    </ul>
</div>
