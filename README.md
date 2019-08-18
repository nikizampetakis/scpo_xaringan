# scpo_xaringan

Minimalist `R` xaringan theme for html presentations using ScPo style/colors.

## Examples

Example presentation at [https://scpoecon.github.io/scpo_xaringan/]( https://scpoecon.github.io/scpo_xaringan/). 

## Usage

just fork this and edit the front-matter YAML at the start of your Rmd file containing your presentation.


```
---
title: "your title"
subtitle: "subtitle"
author: "Your name"
date: "SciencesPo Paris </br> `r Sys.Date()`"
output:
  xaringan::moon_reader:
    lib_dir: libs
    css: [default, "scpo.css", "scpo-fonts.css"]
    nature:
      beforeInit: ["../js/ru_xaringan.js"]
      highlightStyle: github
      highlightLines: true
      countIncrementalSlides: false
      ratio: "16:9"
    includes:
      in_header: "./libs/partials/header.html"
---
```
