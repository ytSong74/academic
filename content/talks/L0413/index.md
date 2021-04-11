---
title: "Building Systems to Enable Spatial Data Science at Scale"
summary: "Mohamed Sarwat, Arizona State University" 
tags:
- Other
- Upcoming
date: "2021-04-13T09:42:37-04:00"

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
#url_video: "https://lecturerecording.umiacs.io/recordings/Lec0401.mp4"

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
#slides: example
---
**Date and Time of the talk:** April 13 2021, 9:30 AM EDT

## Information of the Speaker 
**Mohamed Sarwat, Arizona State University** 

Mohamed Sarwat is an assistant professor of computer science at
Arizona State University. Dr. Sarwat is a recipient of the 2019
National Science Foundation CAREER award and was named an Early Career
Distinguished Lecturer by the IEEE Mobile Data Management community in
June 2019. His general research interest lies in developing robust and
scalable data systems. The outcome of his research has been recognized
by two best research paper awards in the IEEE International Conference
on Mobile Data Management (MDM 2015) and the International Symposium
on Spatial and Temporal Databases (SSTD 2011), a best of conference
citation in the IEEE International Conference on Data Engineering
(ICDE 2012) as well as a best vision paper award (3rd place) in SSTD
2017. Besides impact through scientific publications, Mohamed is also
the co-architect of several software artifacts, which include
GeoSpark (a scalable system for processing big geospatial data) that
is being used by major tech companies such as Uber, Facebook and
MoBike. Dr. Sarwat spent the summers of 2011 and 2012 at NEC
laboratories and Microsoft Research Redmond, respectively. He is an
associate editor for the GeoInformatica journal and has served as an
organizer / reviewer / program committee member for major data
management and spatial computing venues.

## Abstract
In the last 20 years, geospatial data (extracted from GPS
traces, geo-tagged social media, weather maps, natural disasters,
satellites imagery, and epidemic situations) has become wildly
ubiquitous. That led to the rise of spatial data science as a field,
which usually refers to extracting meaningful information from
geospatial data. However, the lack of scalability and interactivity in
state-of-the-art spatial data systems makes it extremely difficult for
a data scientist to store, retrieve, explore, analyze, visualize and
learn from large-scale geospatial data.

In this talk, I will first shed light on Apache Sedona (formerly named
GeoSpark), an open source data system that builds upon the core engine
of Apache Spark to efficiently process large-scale geospatial data in
a cluster computing environment. Internally, Sedona represents
geospatial data as a SpatialRDD, which is tailored for Apache Spark
in-memory data processing paradigm. Sedona allows users to write their
spatial data processing tasks in Spatial SQL, compiles the input SQL
into a set of optimized SpatialRDD operations, and finally executes
such operations in the cluster.
Since a data scientist many times applies the analysis to only a
subset of the entire database, I will give an overview of Hippo a
lightweight indexing scheme that outperforms de-facto database indexes
such B-tree and R-tree in terms of storage and maintenance overhead,
while still executing range queries (to retrieve a subset of the data)
at a comparative performance to such in
dexes. Furthermore, a data scientist may sometimes allow for a slight
trade-off between the accuracy and scalability of the analysis. To
allow for such trade-off, I will present a sampling middleware system
called Tabula, which sits between the data system and the data science
tool (such as Tableau) to make the inherently iterative
human-in-the-loop analysis process more seamless and
interactive. Finally, I will switch gears a bit to present my future
plan related to spatial data systems support for the Internet of
Things (IoT) and the data science for cities initiative.