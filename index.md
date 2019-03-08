---
layout: home
title: Microservices 2017
feature_image: "/2017/assets/images/andersen_museum.jpg"
image: "/2017/assets/images/andersen_museum.jpg"
excerpt: "The first conference on microservices is a forum for the discussion of all aspects of designing and programming microservice architectures. Both theoretical and experimental contributions are welcome, on topics ranging from formal frameworks to experience reports."
---

<ul class="nav nav-tabs nav-justified">
  <li role="presentation" class="active"><a href="#about">About</a></li>
  <li role="presentation"><a href="#cfp">Call for Papers</a></li>
</ul>

<div class="tab-content">
<div role="tabpanel" class="tab-pane active" id="about">
  
  {% include_relative include_md.html file="subpages/about.md" %}

</div>

<div role="tabpanel" class="tab-pane" id="cfp">

  {% include_relative include_md.html file="subpages/call_for_papers.md" %}

</div>

</div>

<script>
$('.nav-tabs li a').click(function (e){e.preventDefault();$(this).tab('show');})
</script>
