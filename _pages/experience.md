---
layout: page
permalink: /experience/
title: Experience
description:
organizations: [
  {
    company: Palantir Technologies,
    role: Forward Deployed Software Engineer Intern,
    timeline: Summer 2020 & Summer 2021,
    description: "At Palantir, I worked on large scale data integration and cleaning by writing transforms for big data, and subsequently utilized the cleaned data to build models and workflows for a partner client. A significant portion of my role was to demo those workflows to clients and guide them through user adoption, all while continuing to finetune the product from a software perspective."
  },
  {
    company: AV Machine Learning Research,
    role: ML Research Assistant,
    timeline: 2019 - Present,
    description: "My research team and I have worked to develop generators for images of terrain. To train the model, we first utilized a webscraper to harvest images of different types of terrain from Google images. Using these images, we trained a convolutional neural network to classify an icy road from other types of terrain. From there, we tuned a generative adversarial network to produce new images of icy roads, effectively testing the accuracy of the CNN. I am currently working on a novel approach to apply generic feature transfer (summer to winter) optimized for few shot learning to a small input dataset of images. I'm currently experimenting with cycle-consistency loss and PatchNCE loss to preserve the input feature mapping while training towards a target domain, while utilizing a pyramid GAN structure to facilitate few-shot learning."
  },
  {
    company: Nexecon Consulting Group,
    role: "Project Manager | Analyst",
    timeline: 2019 - Present,
    description: "With Nexecon Consulting Group, my work as an analyst has allowed me to partner with several high-profile Fortune 500 clients. In one of these projects, I developed a software tool to minimize delays at an international airport by tracking previous flight data and predicting delay chance percentages for future flights, using parameters such as the gate layout. My team and I developed back-end logic as well as a front-end service in React. Most recently, I've worked as the project manager of a team aiming to aide an early-stage start-up in their market research and user acquisition."
  },
  {
    company: Ford Motor Company,
    role: "Software Engineer Intern",
    timeline: Summer 2019,
    description: "During my time at Ford, I built iOS and Android applications that could control automobile functions remotely, such as starting and stopping vehicles. The applications both utilized OAuth security measures and stored accounts and preferences locally on a device to protect privacy. They are now used internally to help developers find bugs in different Ford servers, and are used externally to showcase Ford API functionalities to potential clients."
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
      </div>
    </div>
  {% endfor %}

</div>
