---
layout: default
title: Services
---

<section>
  <h3>Conditions</h3>

  <ul>
    {% for condition in site.data.conditions %}
      <li>{{ condition.title }}</li>
    {% endfor %}
  </ul>
</section>

<section>
  <h3>Treatments</h3>

  <ul>
    {% for treatment in site.data.treatments %}
      <li>{{ treatment.title }}</li>
    {% endfor %}
  </ul>
</section>

<section>
  <h3>What is Dry Needling?</h3>

  <p>
    Dry needling is a technique used by physical therapists that uses needles to stimulate muscle trigger points in order to help heal and rehabilitate dysfunctional muscles and the surrounding area. Studies have shown dry needling is an effective pain relief treatment and also leads to increased muscle performance. Talk to your physical therapist today to find out if dry needling is a treatment option for you!
  </p>
</section>