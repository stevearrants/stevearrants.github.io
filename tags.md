---
layout: page
title: 'Tag Index'
---
 
<style>
.tag-btn {
  background-color: #2D6A4F !important;
  border-color: #2D6A4F !important;
  color: #fff !important;
  margin: 0.25rem;
}
.tag-btn:hover {
  background-color: #1A5C3A !important;
  border-color: #1A5C3A !important;
  color: #fff !important;
  text-decoration: none;
}
.tag-btn i {
  color: #fff !important;
}
#full-tags-list h2.linked-section {
  color: #2D6A4F;
  font-size: 1.2rem;
  margin-top: 2rem;
  border-bottom: 2px solid #E4EAE5;
  padding-bottom: 0.4rem;
}
#full-tags-list h2.linked-section i {
  color: #2D6A4F;
}
.tag-entry {
  padding: 0.4rem 0;
  border-bottom: 1px solid #F0F0F0;
}
.tag-entry a {
  color: #1A6FA8;
}
.entry-date {
  font-size: 0.82rem;
  color: #888;
}
</style>
 
{% assign date_format = site.date_format | default: "%B %-d, %Y" %}
 
{%- capture site_tags -%}
  {%- for tag in site.tags -%}
    {{- tag | first -}}{%- unless forloop.last -%},{%- endunless -%}
  {%- endfor -%}
{%- endcapture -%}
{%- assign tags_list = site_tags | split:',' | sort -%}
 
{%- for tag in tags_list -%}
  <a href="#{{- tag -}}" class="btn btn-primary tag-btn"><i class="fas fa-tag" aria-hidden="true"></i>&nbsp;{{- tag -}}&nbsp;({{site.tags[tag].size}})</a>
{%- endfor -%}
 
<div id="full-tags-list">
{%- for tag in tags_list -%}
  <h2 id="{{- tag -}}" class="linked-section">
    <i class="fas fa-tag" aria-hidden="true"></i>
    &nbsp;{{- tag -}}&nbsp;({{site.tags[tag].size}})
  </h2>
  <div class="post-list">
    {%- for post in site.tags[tag] -%}
      <div class="tag-entry">
        <a href="{{ post.url | relative_url }}">{{- post.title | strip_html -}}</a>
        <div class="entry-date">
          <time datetime="{{- post.date | date_to_xmlschema -}}">{{- post.date | date: date_format -}}</time>
        </div>
      </div>
    {%- endfor -%}
  </div>
{%- endfor -%}
</div>
