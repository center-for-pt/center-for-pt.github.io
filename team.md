---
layout: default
title: Team
---

<section>
  <h2>
    Get to know our talented Richmond, VA physical therapists!
  </h2>

  <div>
    {% for staff_member in site.staff_members %}
      <div>
        <h3>
          <a href="/website{{ staff_member.url }}">
            {{ staff_member.name }}
          </a>
        </h3>
        <img alt="{{ staff_member.name }}" src="/website/assets/images/staff_members/{{ staff_member.slug }}-small.jpg" />
        <p>{{ staff_member.qualifications }}</p>
      </div>
    {% endfor %}
  </div>
</section>