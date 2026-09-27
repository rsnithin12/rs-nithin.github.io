---
show: true
width: 4
date: 2023-01-12 00:01:00 +0800
---

<!-- Conferences Attended -->
<div>
  <div id="conferenceCarousel"
       class="carousel slide"
       data-ride="carousel"
       data-interval="2000">
    <div class="carousel-inner">
      <div class="carousel-item active">
        <img
          src="{{ '/assets/images/covers/pre-1_certificate.jpg' | relative_url }}"
          class="d-block w-100 rounded-xl-top"
          style="height: 300px; object-fit: contain;">
      </div>
      <div class="carousel-item">
        <img
          src="{{ '/assets/images/covers/pre-2_certificate.jpg' | relative_url }}"
          class="d-block w-100 rounded-xl-top"
          style="height: 300px; object-fit: contain;">
      </div>
      <div class="carousel-item">
        <img
          src="{{ '/assets/images/covers/pre-3_certificate.jpg' | relative_url }}"
          class="d-block w-100 rounded-xl-top"
          style="height: 300px; object-fit: contain;">
      </div>
    </div>
    <!-- Previous arrow -->
    <button class="carousel-control-prev"
            type="button"
            data-target="#conferenceCarousel"
            data-slide="prev">
      <span class="carousel-control-prev-icon" ></span>
      <span class="sr-only">Previous</span>
    </button>
    <!-- Next arrow -->
    <button class="carousel-control-next"
            type="button"
            data-target="#conferenceCarousel"
            data-slide="next">
      <span class="carousel-control-next-icon" ></span>
      <span class="sr-only">Next</span>
    </button>
  </div>

  <div class="card-body">
    <h5 class="card-title">Conferences attended</h5>
    <p class="card-text">
      List of conferences with presentations attended.
    </p>
    <p class="card-text">
      <small>
        <a href="{{ '/publications' | relative_url }}">
          See Publications!
        </a>
      </small>
    </p>
  </div>
</div>
