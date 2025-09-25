---
title: "Portfolio of Professional Documents"
excerpt: "A collection of documents showcasing technical communication and project analysis skills."
collection: portfolio
permalink: /portfolio/
author_profile: true
---

Here are documents that showcase my ability to communicate complex technical information clearly and professionally.

---

## Project Retrospective: A Post-Mortem of the Spotify Wrapped Replica

**Project:** Spotify Wrapped Replica Android App  
### Project Overview

This project's goal was to develop a full-stack Android application that emulated the core functionality of Spotify's annual "Wrapped" feature. Over a 10-week agile development cycle, our team of six successfully designed, built, and tested an app that allowed users to authenticate with their Spotify accounts and view personalized data visualizations of their listening habits. As the Scrum Master and a lead backend developer, my role was to facilitate our agile workflow and architect the backend infrastructure.

### What Went Well

* **Agile Workflow & Team Collaboration:** Our commitment to the Scrum framework was a major success. Daily stand-ups kept us synchronized, and sprint retrospectives allowed us to adapt quickly. Team morale remained high, and communication was consistently open and constructive.
* **Rapid Prototyping with Firebase:** Choosing Firebase for our backend proved to be an excellent decision. Its real-time database and straightforward authentication APIs allowed us to build and test our backend logic in a fraction of the time it would have taken with a traditional SQL setup.
* **Clear Division of Roles:** From the outset, we established clear ownership over different parts of the application (Frontend UI, Backend API, Database, and QA). This specialization allowed team members to work efficiently and become experts in their respective domains.

### What Could Be Improved

* **Initial Underestimation of UI Complexity:** During our initial sprint planning, we underestimated the effort required to create polished and animated UI components. This led to a crunch period in the final sprints to meet our aesthetic goals.
* **API Rate Limiting Challenges:** We did not initially account for Spotify's strict API rate limits during development, which caused several temporary lockouts. We eventually implemented a caching layer, but this should have been identified during the initial design phase.

### Key Learnings

This project provided invaluable lessons in both technical execution and team leadership. My primary takeaway as a leader was the immense value of creating psychological safety, where team members felt comfortable admitting mistakes. Technically, I learned the critical importance of designing a **data model optimized for read-heavy operations** in a NoSQL environment to ensure a responsive user experience.

