---
# Mr. Green Jekyll Theme - v1.1.0 (https://github.com/MrGreensWorkshop/MrGreen-JekyllTheme)
# Copyright (c) 2022 Mr. Green's Workshop https://www.MrGreensWorkshop.com
# Licensed under MIT

layout: default
# Links page
---
{%- include multi_lng/get-lng-by-url.liquid -%}
{%- assign lng = get_lng -%}



<div class="multipurpose-container links-heading-container">
  <a href="JikC.github.io/_data/owner/cv.pdf" target="_blank">My CV.</a>
</div>


{% with pdf_file = "_data/owner/cv.pdf" %}

{% set solid_filepdf = '<i class="fas fa-file-pdf"></i>' %}
{% set empty_filepdf = '<i class="far fa-file-pdf"></i>' %}

## Example: Embedding a PDF file

<object data="{{ pdf_file }}" type="application/pdf">
    <embed src="{{ pdf_file }}" type="application/pdf" />
</object>

## Example: Creating a link to a PDF file

# <a href="{{ pdf_file }}" class="image fit">{{ solid_filepdf }}</a>

{% endfor %}
