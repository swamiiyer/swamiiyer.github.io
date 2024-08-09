---
permalink: "/faq.html"
layout: page
title: FAQ
order: 5
---

<div class="aside">
    <div class="container-fluid">
	{% for item in site.data.faqs %}
  	  <div class="panel">
		<div class="panel-heading" data-toggle="{{forloop.index}}"> 	
			<a href="javascript:void(0)" data-toggle="{{forloop.index}}" href="#">Q{{forloop.index}}. {{item.title}}</a>
		</div>
		<div class="panel-body hidden-element" data-body="{{forloop.index}}"> 
            {{item.body}}
		</div>
	  </div>
      <br/>
	{% endfor %}
</div>
</div>
<script src="/public/collapse.js"></script>
