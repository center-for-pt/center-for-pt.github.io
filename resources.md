---
layout: default
title: Resources
---

<section>
  <h3>Accepted Insurances</h3>

  <p>We accept the following insurances for treatment. Please contact us if you have any questions.</p>

  <ul>
    {% for insurance in site.data.insurances %}
      {% if insurance.accepted %}
        <li>
          {{ insurance.title }}
        </li>
      {% endif %}
    {% endfor  %}
  </ul>

  <p>We <strong>do not</strong> accept:</p>

  <ul>
    {% for insurance in site.data.insurances %}
      {% unless insurance.accepted %}
        <li>
          {{ insurance.title }}
        </li>
      {% endunless %}
    {% endfor  %}
  </ul>
</section>

<section>
  <h3>Patient Forms</h3>

  <p>The following forms are available as downloadable documents. Please print those that apply to you, fill them out and bring them to your initial evaluation.</p>

  <ul>
    {% for patient_form in site.data.patient_forms %}
      <li>
        <a href="{{ patient_form.url }}" target="_blank">
          {{ patient_form.title }}
        </a>
      </li>
    {% endfor %}
  </ul>
</section>

<section>
  <h3>Patient FAQ</h3>

  <ul>
    {% for faq in site.data.faq %}
    <li>
      <details>
        <summary>
          {{ faq.q }}
        </summary>

        {{ faq.a }}
      </details>
    </li>
    {% endfor %}
  </ul>
</section>