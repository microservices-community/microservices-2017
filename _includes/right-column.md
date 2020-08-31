<div class="panel panel-primary">
<div class="panel-heading">
<strong>Important Dates</strong>
</div>
<ul class="list-group">

<li class="list-group-item">
<p>
<del>Fri 1</del> <strong>Mon 4 Sept. 2017, 12 a.m.</strong> (Ext'd)
<span data-toggle="tooltip" title="Timezone: CET (UTC+1h)">
<span class="glyphicon glyphicon-time"></span>
</span>
</p>
<p>Paper Submission Deadline</p>
</li>

<li class="list-group-item">
<p><strong>Fri 15 Sept. 2017</strong>
<span data-toggle="tooltip" title="Timezone: AoE (UTC-12h)">
<span class="glyphicon glyphicon-time"></span>
</p>
<p>Author Notification</p>
</li>

<li class="list-group-item">
<p><strong>Mon 9 Oct. 2017</strong>
<span data-toggle="tooltip" title="Timezone: AoE (UTC-12h)">
<span class="glyphicon glyphicon-time"></span>
</p>
<p>Camera-ready</p>
</li>

<li class="list-group-item">
<p><strong>Mon 2 Oct. 2017</strong>
<span data-toggle="tooltip" title="Timezone: AoE (UTC-12h)">
<span class="glyphicon glyphicon-time"></span>
</p>

<p>Registration</p>
</li>

<li class="list-group-item">
<p><strong>25-26 Oct. 2017</strong>
<span data-toggle="tooltip" title="Timezone: CET (UTC+1h)">
<span class="glyphicon glyphicon-time"></span>
</p>

<p>Conference</p>
</li>
</ul>
</div>

<div class="panel panel-primary">
<div class="panel-heading">
<strong>Social Media</strong>
</div>
<div style="width:99%;" >
<a class="twitter-timeline" data-height="600" href="https://twitter.com/c_microservices">Tweets on Microservices 2017</a> <script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>
</div>
</div>

<div class="panel panel-primary">
<div class="panel-heading">
<strong>Supporters</strong>
</div>
<ul class="list-group">

<li class="list-group-item">
  <img class="img-responsive center-block" src="/2017/assets/images/sdu.png" alt="">
</li>
<li class="list-group-item">
  <img class="img-responsive center-block" src="/2017/assets/images/unibo.png" alt="">
</li>
</ul>
</div>


<style>
  .microservices_community_event {
    line-height: 1.05em;
    text-align: left;
    margin-top: 9px;
  }
</style>

<div class="panel panel-primary">
  <div class="panel-heading">
  <strong>Microservices Community Events</strong>
  </div>
  <ul class="list-group">
  <li class="list-group-item"> 
    <div>Upcoming events</div>
    <div id="microservices_community_events_upcoming"></div>
  </li>
  <li class="list-group-item"> 
    <div>Latests past events</div>
    <div id="microservices_community_events_past"></div>
  </li>
  </div>
</div>

<script>
function microservices_community_events( data ){
  const upcoming = $( "#microservices_community_events_upcoming" )
  data.upcoming.forEach( element => {
    upcoming.append( 
      `<div>
      <a target="_blank" href="${ element.link }">
        <div class="microservices_community_event" >${ element.title }</div>
      </a>
      </div>` )
  });
  const past = $( "#microservices_community_events_past" )
  data.past.forEach( ( element, index ) => {
    if( index > 2 ){ return }
    past.append( 
      `<div>
      <a target="_blank" href="${ element.link }">
        <div class="microservices_community_event" >${ element.title }</span>
      </a>
      </div>` )
  });
}
$( document ).ready( () => {
  const url = "https://www.microservices.community/events.json"
  $.ajax({
    url: url,
    jsonp: "microservices_community_events",
    dataType: "jsonp"
  })
})

<script>
$(document).ready(function(){$('[data-toggle="tooltip"]').tooltip();});
</script>
