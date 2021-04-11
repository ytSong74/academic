---
title: "QARTA: An ML–Based System for Accurate Map Services"
subtitle: In collaboration with the UMD Center for Machine Learning
summary: Ahmed Eldawy, University of California Riverside
tags:
- Machine Learning
date: "2021-04-06T09:42:37-04:00"

# Optional external URL for project (replaces project detail page).
#external_link: ""

# image:
#   caption: Photo by rawpixel on Unsplash
#   focal_point: Smart

# links:
# - icon: twitter
#   icon_pack: fab
#   name: Follow
#   url: https://twitter.com/georgecushen
# url_code: ""
# url_pdf: ""
# url_slides: ""
url_video: "https://spatialhandling-lectureseries.umiacs.io/recordings/Lec0406.mp4"

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
#slides: example
---
**Date and Time of the talk:** April 06 2021, 9:30 AM EDT

## Information of the Speaker 
 **Mohamed Mokbel, University of Minnesota** 
 
A Ph.D. graduate of Purdue University, Mohamed Mokbel is a Professor at the University of Minnesota. Prior roles while on leave/sabbatical from UMN include Chief Scientist of Qatar Computing Research Institute, Founding Technical Director of the GIS Technology Innovation Center in Saudi Arabia, and multiple times Visiting Researcher at Microsoft Research, USA. His current research interests focus on building systems for big spatial data and applications. His research work has been recognized by the NSF CAREER Award, VLDB 10-years Best Paper Award, and four conference Best Paper Awards. Mohamed is the past elected Chair of ACM SIGSPATIAL, current Editor-in-Chief for Springer Distributed and Parallel Databases Journal, and he is on the editorial board of ACM Books, ACM TODS, VLDB Journal, ACM TSAS, and GeoInformatica journals. He has served as PC Co-Chair for ACM SIGMOD, ACM SIGSPATIAL, and IEEE MDM. He is an IEEE Fellow and an ACM Distinguished Scientist.

## Abstract
Maps services (e.g., routing and store finding) are ubiquitous in widely used applications including navigation systems, ride sharing, and items/food delivery. There are plenty of efforts dedicated to supporting such services through designing more efficient algorithms, e.g., efficient shortest path and range queries. We believe that efficiency is no longer a bottleneck to these map services. Instead, it is the accuracy of the underlying road network and query result. In this talk, we present QARTA, an open-source full-fledged system for highly accurate and scalable map services. QARTA employs machine learning techniques to construct its own highly accurate map, not only in terms of map topology but more importantly, in terms of edge weights. QARTA also employs machine learning techniques to calibrate its query answers based on contextual information, including transportation modality, location, and time of day/week.