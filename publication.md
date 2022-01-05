---
layout: page
title: Publication
permalink: /publication/
years: [2022, 2021, 2020, 2019, 2018, 2017, 2016, 2015, 2014, 2013, 2012, 2011]
---

<style type="text/css">
.btnPub--url {
	background:linear-gradient(to bottom, #74ad5a 5%, #68a54b 100%);
	background-color:#74ad5a;
	border-radius:3px;
	border:1px solid #3b6e22;
	display:inline-block;
	cursor:pointer;
	color:#ffffff;
	font-family:Verdana;
	font-size:10px;
	padding:1px 5px;
	text-decoration:none;
}
.btnPub--url:hover {
	background:linear-gradient(to bottom, #68a54b 5%, #74ad5a 100%);
	background-color:#68a54b;
}
.btnPub--url:active {
	position:relative;
	top:1px;
}
.btnPub--BibTex {
	background:linear-gradient(to bottom, #007dc1 5%, #0061a7 100%);
	background-color:#007dc1;
	border-radius:3px;
	border:1px solid #124d77;
	display:inline-block;
	cursor:pointer;
	color:#ffffff;
	font-family:Verdana;
	font-size:10px;
	padding:1px 5px;
	text-decoration:none;
}
.btnPub--BibTex:hover {
	background:linear-gradient(to bottom, #0061a7 5%, #007dc1 100%);
	background-color:#0061a7;
}
.btnPub--BibTex:active {
	position:relative;
	top:1px;
}

.btnPub--preprint {
	background:linear-gradient(to bottom, #f24537 5%, #c62d1f 100%);
	background-color:#f24537;
	border-radius:3px;
	border:1px solid #d02718;
	display:inline-block;
	cursor:pointer;
	color:#ffffff;
	font-family:Verdana;
	font-size:10px;
	padding:1px 5px;
	text-decoration:none;
	text-shadow:0px 1px 0px #810e05;
}
.btnPub--preprint:hover {
	background:linear-gradient(to bottom, #c62d1f 5%, #f24537 100%);
	background-color:#c62d1f;
}
.btnPub--preprint:active {
	position:relative;
	top:1px;
}

.raw-bibtex {
	background-color:#eeeeee;
    font-size: 12px;
}

</style>

You can also find my articles on my [Google Scholar profile](https://scholar.google.com/citations?user=RE9h8MsAAAAJ&hl=en).

{% for y in page.years %}
  <h3 id="{{y}}" class="pubyear">{{y}}</h3>
  {% bibliography -q @*[year={{y}}]* %}
{% endfor %}
