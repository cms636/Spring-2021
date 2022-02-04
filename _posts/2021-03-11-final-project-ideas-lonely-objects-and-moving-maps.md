---
layout: post
published: true
category: updates
title: 'Final project ideas: lonely objects and moving maps'
author: Justin Blinder
tags: ''
---
**Update:**
After learning more about other folks ideas, I saw some overlapping themes with Sarah, Mulan, and Delace's concepts in terms of adding extra context/ content to collections and thinking about how visitors traverse museums. One variation on the idea I had of determining popular works via visitor tracking is using online, social representations of museums as a way of curating new ("off the beaten path") experiences for visitors. Many MFA visitors post photos of works they viewed on Instagram and tag the museum. I think using this data to determine artists, works, time periods, etc. that are shared the most could be an interesting way of uncovering under-explored/ unshared areas in the museum. This information could then be used to guide new/ returning visitors towards these areas. This could be in the form of an interactive map, brochure, game, etc. and also provide additional media/ content to incentivize exploration. I'm also curious if these Instagram posts could be recontextualized within the museum.

---

I came up with two rough ideas that could be explored at an institution with a diverse collection, like the MFA, the Getty museum, or the Met.

**What are the least viewed pieces at museums?**  

Museums often highlight specific works in their permanent collections, rotating exhibitions, and promotional materials. Certain museums are often linked to works in their permanent collection: the Louvre and the Mona Lisa, Neues Museum (Berlin) and the Nefertiti Bust, the blue whale model at the American Museum of Natural History. However, this begs the question-- Which works thus remain neglected, and fall outside the periphery of typical visitor interest? Poor placement, uninteresting aesthetics/ content/ context for a visitor, and bad art (I’m kidding!) could all be contributing factors to why certain pieces aren’t viewed as much as others. If so-called “blockbuster” works are now sometimes Instagram props for digital experiences, can digital tools actually reconnect visitors to look at and engage with art, rather than photographing it, as their museum experience?

This project seeks to understand visitor attention toward specific pieces in a museum, reveal patterns as to why certain works are engaged with more than others, and guide viewers towards less-viewed works. At a (super) high level, it addresses the following questions: Are there patterns between which works are viewed more often and which works are less viewed? Are there patterns between artists’ demographic profiles, geography, content, style/ school among highly visited/ neglected works? How can neglected works be given more relevance?

This project would be ideally be designed for two specific audiences: Museum curators and researchers to 1) study what works interests viewers the most 2) collect analytics about visitor traffic throughout exhibits 3) reveal patterns vis-a-vis (un)popular works; Visitors to 1) highlight works/ areas that they might normally miss when following the traditional paths throughout the museum 2) have an opportunity to view objects/ works by artists that are scarcely documented/ photographed and hard to find outside of the museum.

The technical implementation is pretty open-ended. One literal and granular approach would be to: 1) Create a dataset with metadata about each work in a museum including information about the creator, place of origin, date, and content features (e.g. spoon, horse, etc.). 2) Build a tracking system to determine viewer presence and duration in front of a specific work (computer vision, bluetooth/ wifi beacon sniffing, infrared/ ultrasonic sensors, or QR codes). 3)Analyze the visitor engagement for each work and the metadata associated with the work to detect patterns (example: paintings of cats between 1700-1900 have the most traffic) 4) Create a tool/ app/ intervention that guides visitors towards lesser viewed works, And/ or create a tool for museum staff to make sense of visitor traffic in relation to types of works. (example: you might want to check out this painting of a dog from the early 1400s). An alternative approach to #2 could be to analyze social media posts tagged/ associated with the museum to see which works are shared the most.

I think web development (HTML/CSS/Javascript), data science (NLP, classification), and/ or UX/ UI design skills would all be relevant. In the example above, the tracking system could be simulated/ fake dataset.

Many museums have security cameras, and a real-time tracking systems (that doesn’t save footage) could live on top of this existing infrastructure. Still, tracking visitors via cameras, Bluetooth/ WiFi beacon sniffing, raises privacy concerns that should be considered in the course of the project, or even before, to inform whether the project should be explored.

**Rethinking the Museum Map**  

Planning a visit to a large museum with an extensive permanent collection can be overwhelming. Museum maps typically provide a spatial reference that’s only segmented by collection, current exhibits, time period, geography, etc. They also segment the museum statically, often treating individual rooms as sections of larger collections or wings rather than their own unique spaces. How can museums be redefined spatially without changing the space itself? How can visitors navigate museums in ways that’s specifically curated based on their own interests?

This project explores creating dynamic, personalized maps of museums based on the features and information embedded in the works in a collection. Instead of choosing their path based on traditional descriptions and groupings, visitors can select different features they’re interested in to inform their route. For example, all monotone paintings, pictures containing cats, or works created when an artist was in their 20s whose name begins with the letter "H". Based on these selections, a new map is generated for the visitor showing them their curated path throughout the museum, across different rooms, exhibits, floors, etc. 

Given the immmense amount of planning and consideration that goes into museum architecture, I think it's important to contextualize this tool within the map itself rather than creating an entirely new one. This tool uses the existing physical museum map as a canvas for an interactive AR experience that visualizes a personlized, curated route. Visitors first visit a website on their phone or an interactive display at the museum where they explore the archive via various filters, features, etc.. Once they've selected their interests, the app generates a route creates a shortened url (that can be scanned as a QR code) which directs to an mobile AR app. Visitors scan their personal map (or one on a wall) and see their route overlaid, which can provide additional details about a work once a user is within proximity.

This tool would ideally be designed to allow visitors to navigate the museum in ways based on their own interests. However, this information could also be useful for the museum to discover their visitor’s nuanced interests and how that relates to the location of works. Some examples of analyzing images/ grouping/ filtering objects include clustering images based on visual or content similarity (e.g. blue paintings, pictures of cats), creating topics from works across collections (e.g. all works related to birth/ death), and other approaches. Each path would be saved, and when a new visitor enters a similar criteria the application could suggest similar paths/ works they might be interested in.

I think web development (HTML/CSS/Javascript), data science (NLP, classification), data visualization, web scraping, AR experience, and/ or UX/ UI design skills would all be relevant (but absolutely neccessary to create a prototype.)

[Example image](https://i.imgur.com/s10npmk.png)
