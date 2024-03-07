---
layout: default
title: Executive Committee
date: 2022-09-01
author: Your Name
description: Information about the executive committee of Zimsa Website.
---

<div class="container">
    <!-- Three columns of text below the carousel -->
  <div class="row">

    {% for member in site.data.execcommittee %}
        <div class="col-lg-4 text-center">
            <img src="{{ member.image }}" alt="Profile Picture" class="img-thumbnail rounded-circle mx-auto d-block" style="max-width:350px;">
            <h3 class="fw-normal">{{ member.name }}</h3>
            <h5>{{ member.position }}</h5>
            
            <div class="d-flex justify-content-between align-items-center">
  <a href="tel:{{ member.phone-number }}" class="text-dark me-3 fs-3">
    <i class="bi bi-telephone-fill"></i>
  </a>
  <a href="https://wa.me/{{ member.phone-number }}" class="text-dark me-3 fs-3">
    <i class="bi bi-whatsapp"></i>
  </a>
  <a href="mailto:{{ member.email }}" class="text-dark me-3 fs-3">
    <i class="bi bi-envelope"></i>
  </a>
  <a href="{{ member.linkedin }}" class="text-dark me-3 fs-3">
    <i class="bi bi-linkedin"></i>
  </a>
</div>
</div>
    {% endfor %}
  </div><!-- /.row -->
</div>