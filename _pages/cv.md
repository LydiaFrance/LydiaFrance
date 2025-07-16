---
layout: default
permalink: /cv/
title: cv
nav: true
nav_order: 5
description: This is a description of the page. You can modify it in '_pages/cv.md'. You can also change or remove the top pdf download button.
---

<style>
/* Resume-specific styles extracted from resume.html */
@font-face {
  font-family: 'Josefin Sans';
  font-style: normal;
  font-weight: 300;
  src: local('Josefin Sans Light'), local('JosefinSans-Light'), url(https://fonts.gstatic.com/s/josefinsans/v14/Qw3FZQNVED7rKGKxtqIqX5Ecpl5te10k.ttf) format('truetype');
}

@font-face {
  font-family: 'Josefin Sans';
  font-style: normal;
  font-weight: 700;
  src: local('Josefin Sans Bold'), local('JosefinSans-Bold'), url(https://fonts.gstatic.com/s/josefinsans/v14/Qw3FZQNVED7rKGKxtqIqX5Ectllte10k.ttf) format('truetype');
}

@font-face {
  font-family: 'Lato';
  font-style: italic;
  font-weight: 300;
  src: local('Lato Light Italic'), local('Lato-LightItalic'), url(https://fonts.gstatic.com/s/lato/v16/S6u_w4BMUTPHjxsI9w2_Gwfo.ttf) format('truetype');
}

@font-face {
  font-family: 'Lato';
  font-style: italic;
  font-weight: 400;
  src: local('Lato Italic'), local('Lato-Italic'), url(https://fonts.gstatic.com/s/lato/v16/S6u8w4BMUTPHjxsAXC-v.ttf) format('truetype');
}

@font-face {
  font-family: 'Lato';
  font-style: italic;
  font-weight: 700;
  src: local('Lato Bold Italic'), local('Lato-BoldItalic'), url(https://fonts.gstatic.com/s/lato/v16/S6u_w4BMUTPHjxsI5wq_Gwfo.ttf) format('truetype');
}

@font-face {
  font-family: 'Lato';
  font-style: normal;
  font-weight: 300;
  src: local('Lato Light'), local('Lato-Light'), url(https://fonts.gstatic.com/s/lato/v16/S6u9w4BMUTPHh7USSwiPGQ.ttf) format('truetype');
}

@font-face {
  font-family: 'Lato';
  font-style: normal;
  font-weight: 400;
  src: local('Lato Regular'), local('Lato-Regular'), url(https://fonts.gstatic.com/s/lato/v16/S6uyw4BMUTPHjx4wXg.ttf) format('truetype');
}

@font-face {
  font-family: 'Lato';
  font-style: normal;
  font-weight: 700;
  src: local('Lato Bold'), local('Lato-Bold'), url(https://fonts.gstatic.com/s/lato/v16/S6u9w4BMUTPHh6UVSwiPGQ.ttf) format('truetype');
}

/* Resume styling */
#resume {
  background: white;
  font-family: "Lato", Helvetica, Arial, sans-serif;
  font-weight: 400;
  color: #222;
  margin: 0 auto;
  max-width: 8.5in;
  min-height: 11in;
  padding: 0.5in 0.7in;
  box-shadow: 0 4px 8px rgba(0,0,0,0.1);
}

#resume h1 {
  font-family: "Josefin Sans", Helvetica, Arial, sans-serif;
  font-weight: 700;
  font-size: 28px;
  letter-spacing: 1px;
  margin: 0;
}

#resume h2 {
  font-family: "Josefin Sans", Helvetica, Arial, sans-serif;
  font-weight: 300;
  font-size: 16px;
  letter-spacing: .5px;
}

#resume h3 {
  font-family: "Lato", Helvetica, Arial, sans-serif;
  font-weight: 300;
  font-size: 14px;
  letter-spacing: .4px;
}

#resume h3.bold {
  font-weight: 700;
}

#resume h4 {
  font-family: "Lato", Helvetica, Arial, sans-serif;
  font-weight: 300;
  font-size: 12px;
}

#resume h4.bold {
  font-weight: 700;
}

#resume h5 {
  font-family: "Lato", Helvetica, Arial, sans-serif;
  font-weight: 300;
  font-size: 11px;
}

#resume h5.italic {
  font-style: italic;
}

#resume h6 {
  font-family: "Lato", Helvetica, Arial, sans-serif;
  font-weight: 400;
  font-size: 10px;
}

#resume a {
  color: inherit;
  text-decoration: inherit;
}

#resume a:hover {
  color: #b509ac;
}

#resume a .fa-external-link {
  font-size: 10px;
  vertical-align: text-top;
}

#resume p,
#resume li {
  font-size: 11px;
}

#resume blockquote {
  font-size: 11px;
  font-family: "Lato", Helvetica, Arial, sans-serif;
  font-weight: 400;
  font-style: italic;
  margin: 10px 25px;
}

#resume em {
  color: #999;
}

#resume ul {
  margin: 10px 0 0;
  -webkit-padding-start: 25px;
}

#resume ul li {
  padding-left: 10px;
}

#resume ul.minimal {
  list-style: none;
  padding: 0;
}

#resume ul.minimal li {
  margin-bottom: 3px;
  padding-left: 0;
}

#resume ul.two-column {
  -webkit-column-count: 2;
  -webkit-column-gap: 28px;
  column-count: 2;
  column-gap: 28px;
}

#resume ul.two-column li {
  padding-left: 0;
}

.resume-header {
  padding-bottom: 20px;
  border-bottom: 4px solid #b509ac;
  margin-bottom: 20px;
}

.profile-header {
  width: 70%;
  float: left;
}

.profile-pic {
  width: 25%;
  float: right;
  text-align: right;
}

.profile-pic img {
  width: 100px;
  height: 100px;
  border-radius: 50%;
  object-fit: cover;
}

.resume-content {
  display: flex;
  gap: 20px;
}

.left-column {
  width: 35%;
}

.right-column {
  width: 65%;
}

.container {
  margin-bottom: 20px;
}

.title h3 {
  margin: 0 0 5px 0;
  font-weight: 700;
  color: #b509ac;
}

.keyline {
  height: 1px;
  background: #ddd;
  margin-bottom: 15px;
}

.info-tag-container {
  display: flex;
  align-items: center;
  margin-bottom: 8px;
}

.info-tag-container i {
  width: 20px;
  color: #b509ac;
  margin-right: 10px;
}

.info-text {
  margin: 0;
  font-size: 10px;
}

.clearfix::after {
  content: "";
  display: table;
  clear: both;
}

.item {
  margin-bottom: 15px;
  page-break-inside: avoid;
}

.item h4 {
  margin: 0 0 5px 0;
  font-weight: 700;
}

.item h5 {
  margin: 0 0 3px 0;
  color: #666;
}

.item .date {
  font-size: 10px;
  color: #999;
  font-style: italic;
}

.item ul {
  margin-top: 5px;
}

.item-details {
  margin-top: 5px;
}

.references-container .item {
  margin-bottom: 10px;
}

.pill {
  display: inline-block;
  background: #f0f0f0;
  padding: 2px 8px;
  margin: 2px;
  border-radius: 10px;
  font-size: 9px;
  color: #666;
}

@media print {
  #resume {
    box-shadow: none;
    margin: 0;
    padding: 0;
  }
}
</style>

<div style="margin-bottom: 2rem;">
  <a href="{{ '/assets/json/resume.html' | relative_url }}" target="_blank" class="btn btn-primary">
    <i class="fa-solid fa-external-link"></i> View Full Resume Page
  </a>
</div>

<!-- Resume content will be embedded here -->
<div id="resume-container">
  <iframe src="{{ '/assets/json/resume.html' | relative_url }}" 
          style="width: 100%; height: 100vh; border: none; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);"
          title="Resume">
  </iframe>
</div>

<noscript>
  <p>If the resume doesn't load above, <a href="{{ '/assets/json/resume.html' | relative_url }}">click here to view it directly</a>.</p>
</noscript>
