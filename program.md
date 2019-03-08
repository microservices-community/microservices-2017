---
title: Program
layout: page
feature_image: "/2017/assets/images/skal_odense.jpg"
---

<div class="alert alert-info" role="alert"> <strong>Heads up!</strong> 

  <p>Please use 
  <span class="glyphicon glyphicon-arrow-right" aria-hidden="true"></span> 
  <a href="http://tinyurl.com/ms-panel-topics">this form</a> 
  <span class="glyphicon glyphicon-arrow-left" aria-hidden="true"></span> 
  to submit topics and question for the October, 26th The Future of Microservices panel.</p>

  <p>Please use 
    <span class="glyphicon glyphicon-arrow-right" aria-hidden="true"></span> 
    <a href="https://goo.gl/forms/BAv09swRBeQGWALO2">this form</a> 
    <span class="glyphicon glyphicon-arrow-left" aria-hidden="true"></span> 
    to sign up for the October, 25th dinner.</p>
</div>


<ul class="nav nav-tabs nav-justified">
  <li role="presentation" class="active">
    <a href="#program">Program</a></li>
  <li role="presentation"><a href="#abstracts">Abstracts</a></li>
  <li role="presentation"><a href="#keynotes">Keynotes</a></li>
</ul>

<div class="tab-content">
<div role="tabpanel" class="tab-pane active" id="program">
  {% include_relative include_md.html file="subpages/program.md" %}
</div>

<div role="tabpanel" class="tab-pane" id="abstracts">
  {% include_relative include_md.html file="subpages/abstracts.md" %}
</div>

<div role="tabpanel" class="tab-pane" id="keynotes" markdown="1">
 
  {% include_relative include_md.html file="subpages/keynotes.md" %}

</div>

<script>
$('.nav-tabs li a').click(function (e){e.preventDefault();$(this).tab('show');})
</script>
