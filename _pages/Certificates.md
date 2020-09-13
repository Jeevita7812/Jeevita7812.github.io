---
permalink: /certificates/
title: "My Certificates"
excerpt: "My certificates for completing coursera courses."
toc: true
---
{% assign certificates = site.static_files | where: "certificate", true %}
{% for certificate in certificates %}
<object data="{{certificate.path}}" type="application/pdf" width="100%" height="100%">
<p>It appears you don't have a PDF plugin for this browser.
No biggie... you can <a href="{{certificate.path}}">click here to
download the PDF file.</a></p>  
</object>
{% endfor %}
