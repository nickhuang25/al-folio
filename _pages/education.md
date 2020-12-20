---
layout: page
permalink: /education/
title: Education
description:
organizations: [
  {
    company: University of Michigan - College of Engineering,
    role: B.S.E Computer Science,
    timeline: 2018 - 2021,
    description: "GPA: 3.83/4.00",
    description2: "Relevant Coursework: Web Systems, Machine Learning, Conversational AI, Data Structures and Algorithms, Computer Organization",
    description3: "Skills and Libraries: Javascript, Python, Flask, Node.js, Java, C, C++, Swift, MATLAB, HTML, CSS, PyTorch, Keras, Tensorflow, Spark"
  },
  {
    company: University of Michigan - Ross School of Business,
    role: Minor in Business,
    timeline: 2019 - 2021,
    description: "Organizations: Nexecon Consulting Group, Alpha Kappa Psi Business Fraternity",
    description2: "Relevant Coursework: Base of the Pyramid: Business Innovation and Social Impact, Marketing, Finance, Accounting"
  },
]
nav: true
---

<div class="experiences">

  {% for org in page.organizations %}
    <hr>
    <div class="expContainer">
      <div class="timeline">
        <p class="time">{{org["timeline"]}}</p>
      </div>
      <div class="expInfo">
        <p class="company">{{org["company"]}}</p>
        <p class="role">{{org["role"]}}</p>
        <p class="description">{{org["description"]}}</p>
        <p class="description">{{org["description2"]}}</p>
        <p class="description">{{org["description3"]}}</p>
      </div>
    </div>
  {% endfor %}

</div>
