---
layout: default
title: Executive Committee
description: Information about the executive committee of Zimsa Website.
image: /assets/img/logos/scome.png
permalink: /nec
---

<div class="container">
  <div class="m-3 align-content-center text-center">
      <h1>2023/2024 National Executive Committee</h1>
      <p>The people you voted for...</p>
    </div>
  <div class="row mt-5">
    {% for member in site.data.execcommittee %}
        <div class="col-lg-4 mb-5">
            <div class="card h-100 shadow border-0">
            <div class="card-body text-center mt-2 px-4 pt-2 rounded-top">
                <img src="{{ member.image }}" alt="Profile Picture" class="img-fluid rounded-circle mx-auto d-block" style="max-width:200px;">
                <h3 class="fw-bold">{{ member.name }}</h3>
                <h5>{{ member.position }}</h5>
            </div>
            <div class="pt-0 bg-transparent">
                <div class="d-flex justify-content-between align-items-center px-4 pb-5">
                <a href="tel:{{ member.phone-number }}" class="text-dark me-1 fs-5"><i class="bi bi-telephone-fill"></i></a>
                <a href="https://wa.me/{{ member.phone-number }}" class="text-dark me-1 fs-5"><i class="bi bi-whatsapp"></i></a>
                <a href="mailto:{{ member.email }}" class="text-dark me-1 fs-5"><i class="bi bi-envelope"></i></a>
                <a href="{{ member.linkedin }}" class="text-dark me-1 fs-5"><i class="bi bi-linkedin"></i></a>
                </div>
            </div>
            </div>
        </div>
    {% endfor %}
  </div>
</div>