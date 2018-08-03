---
layout: post
title:  "LF Mall Project"
date:   2017-07-24
image: "https://chanmi-lee.github.io/images/project-lf.png"
excerpt: "Online e-commerce platform"
tag:
- Java
- Spring framework
- JavaScript
- jQuery
- Thymeleaf
- Oracle
- MySql
---

## Preview
<figure class="half">
{% capture images %}
	{{ site.url }}/images/project-lfmall-pweb.png
	{{ site.url }}/images/project-lfmall-pweb-product.png
{% endcapture %}
{% include gallery images=images caption="Screenshots of LF Mall (pweb)" cols=2 %}
</figure>
<figure class="third">
{% capture images %}
	{{ site.url }}/images/project-lfmall-mweb.png
	{{ site.url }}/images/project-lfmall-mweb-product.png
	{{ site.url }}/images/project-lfmall-mweb-filter.png
{% endcapture %}
{% include gallery images=images caption="Screenshots of LF Mall (mweb)" cols=3 %}
</figure>
<center><b>LF Mall</b> is one of online e-commerce platforms in South Korea.</center><br>

---

### Description
LF Mall has its [web site](https://www.lfmall.com/) and also its [mobile site](https://m.lfmall.com/).
The web/mobile applications is built on Spring framework for handling API requests, with JavaScript/jQuery/Thymeleaf.
This application interacts with ElasticSearch, which requests information from products and those properties like price, brands, colors, and so on. 

<figure class="third">
{% capture images %}
	{{ site.url }}/images/ElasticSearch.png
	{{ site.url }}/images/jQuery.png
	{{ site.url }}/images/Thymeleaf.png
{% endcapture %}
{% include gallery images=images caption="" cols=3 %}
</figure>

---

### Period
* 2017-07 ~ 2018.06 (1 year)

---

### Used skills
`Back-end`
* Java (Spring framework)

`Front-end`
* JavaScript
* jQuery
* Thymeleaf
* HTML & CSS
* JSP

`Database`
* Oracle
* MySql
