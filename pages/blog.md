---
layout: page
permalink: "/blog.html"
title: "Latest news"
description: 'Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum."'
---
<div class="container mt-5 animated fadeInDown">

  	<!-- Grid row -->
    <div class="row">
{% for post in site.posts limit:12 %}
      <!-- Grid column -->
      <div class="col-lg-4 col-md-12 mb-lg-0 mb-4">

        <!-- Card -->
        <div class="card hoverable">

          <!-- Card image -->
          <img class="card-img-top" src="{{post.images}}" alt="Card image cap">

          <!-- Card content -->
          <div class="card-body">

            <!-- Title -->
            <a href="#!" class="black-text">{{ post.title }}</a>
            <!-- Text -->
            <p class="card-title text-muted font-small mt-3 mb-2">{{ post.description }}</p>

            <button type="button" class="btn btn-flat text-primary2 p-0 mx-0"><a href="">Read more</a><i class="fa fa-angle-right ml-2"></i></button>

          </div>

        </div>
        <!-- Card -->

      </div>
      <!-- Grid column -->
      {% endfor %}

    </div>
    <!-- Grid row -->



</div>
