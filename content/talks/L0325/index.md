---
title: "Path and Distance Oracles in Spatial Networks"
summary: Jagan Sankaranarayanan, Google
tags:
- Other
date: "2021-03-25T09:42:37-04:00"

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
**Date and Time of the talk:** March 25 2021, 9:30 AM EDT

## Information of the Speaker 
 **Jagan Sankaranarayanan, Google** 
 
Jagan Sankaranarayanan is a technical lead in the data infrastructure group
at Google. Prior to that, he was the Department Head of Data Management at
NEC Labs America. Jagan got a doctoral degree in Computer Science from the
University of Maryland with Prof. Hanan Samet. His Ph.D. thesis was
nominated for both the ACM Doctoral and Jim Gray dissertation awards by The
University of Maryland. Jagan is a recipient of several awards: Test of
time award from ACM SIGSPATIAL in 2018, Best Paper Awards from ACM SIGMOD
and ACM SIGSPATIAL GIS in 2008 as well as the Best Journal Paper of 2007
Award, ICDE 2009 runner-up, and the Top Cited Award 2005-2010 from
Computers and Graphics Journal. He also received the NEC Invention of the
year (2014), University of Maryland Best Invention of 2009 and a
citizenship award at Google. He has published more than 60 papers and
serves in the editorial board of the Distributed and Parallel Databases
Journal. Recently, he was a program chair of ACM SIGSPATIAL and publicity
chair of ACM SIGMOD.

## Abstract
Spatial networks (e.g., road networks) are general graphs with spatial
information (e.g., latitude/longitude) information associated with the
vertices and/or the edges of the graph. Techniques are presented for query
processing on spatial networks that are based on the observed coherence
between the spatial positions of the vertices and the shortest paths
between them. This facilitates aggregation of the vertices into coherent
regions that share vertices on the shortest paths between them. Using these
frameworks, scalable oracles are conceptualized that can perform a wide
variety of operations such as nearest neighbor finding and distance joins
on large datasets of locations residing on a spatial network. These
frameworks essentially decouple the process of computing shortest paths
from that of spatial query processing as well as also decouple the domain
of the participating objects from the domain of the vertices of the spatial
network. This means that as long as the spatial network is unchanged, the
algorithm and underlying representation of the shortest paths in the
spatial network can be used with different sets of objects.