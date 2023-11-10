---
title: Sec 1 Reg Test Page
permalink: /sec1regtest/
variant: markdown
description: ""
---
  
var&nbsp;acc =&nbsp;document.getElementsByClassName("accordion");  
var&nbsp;i;  
  
for&nbsp;(i =&nbsp;0; i &lt;&nbsp;acc.length; i++) {  
&nbsp; acc\[i\].addEventListener("click",&nbsp;function() {  
&nbsp;&nbsp;&nbsp;&nbsp;this.classList.toggle("active");  
&nbsp;&nbsp;&nbsp;&nbsp;var&nbsp;panel =&nbsp;this.nextElementSibling;  
&nbsp;&nbsp;&nbsp;&nbsp;if&nbsp;(panel.style.maxHeight) {  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;panel.style.maxHeight&nbsp;\=&nbsp;null;  
&nbsp;&nbsp;&nbsp; }&nbsp;else&nbsp;{  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; panel.style.maxHeight&nbsp;\=&nbsp;panel.scrollHeight&nbsp;+&nbsp;"px";  
&nbsp;&nbsp;&nbsp; }  
&nbsp; });  
}  

<style>
.accordion {
  background-color: #eee;
  color: #444;
  cursor: pointer;
  padding: 18px;
  width: 100%;
  border: none;
  text-align: left;
  outline: none;
  font-size: 15px;
  transition: 0.4s;
}

.active, .accordion:hover {
  background-color: #ccc;
}

.panel {
  padding: 0 18px;
  background-color: white;
  max-height: 0;
  overflow: hidden;
  transition: max-height 0.2s ease-out;
}
</style>



<h2>Animated Accordion</h2>
<p>Click on the buttons to open the collapsible content.</p>

<button class="accordion">Section 1</button>
<div class="panel">
  <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
</div>

<button class="accordion">Section 2</button>
<div class="panel">
  <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
</div>

<button class="accordion">Section 3</button>
<div class="panel">
  <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
</div>