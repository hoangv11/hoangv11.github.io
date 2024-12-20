---
layout: project
type: project
image: img/UHSpace.png
title: "UHSpace Data Hub"
date: 2024
published: true
labels:
  - NextJS
  - Firebase
  - AWS
  - LLMs
summary: "Open Data Portal developed by my team for HACC 2024"
---

## Overview

This projects involved recreating Hawaii's Open Source Data Portal, a platform designed to make publicly accessible datasets easy to explore, visualize and manage. The portal allows users to view data and gain much more meaningful insights on data through data visualization charts as well as 24/7 assistance with Uncle HEX, our AI chatbot specialized in reading and analyzing data files such as CSV files. UHSpace also offers a very user friendly interface allowing users to easily navigate through hundred of datasets and saving specfic datasets with a bookmarking feature. The goal was to provide a functional and visually appealing portal to facilitate data accessibility and usage.

## Website Walkthrough

1. Browse through hundreds of diverse data sets and visualize them with our CSV data visualizer.
2. Bookmark data sets that interest you so you can view them later at anytime, anywhere on the application.
3. Access to 24/7 support with our Uncle HEX chatbot. Download the CSV files from the dataset and upload to uncle HEX to gain insights on your data.
4. With the data, use the HEX dashboard, equipped with tools to create your own custom reports. You can also generate graph images using our CSV visualizer.
5. You can upload your reports/projects into our community projects showcase page where anyone can view and interact with the project you made.

## Preview the Website Here

<iframe src="https://uhspace.org/" width="100%" height="600px" frameborder="0" title="HEX"></iframe>

## My Role and Contribution:
As a key contributor to this project, I was responsible for several core aspects of the portal's development. My specific contributions included:

Database Management and CRUD Operations:

Designed and maintained the backend database to support CRUD (Create, Read, Update, Delete) operations for dynamic DataCards.
Implemented optimized queries to fetch and display data efficiently, ensuring minimal latency during user interactions.
Bookmarking Feature:

Built a robust bookmarking system using React hooks like useState and useEffect, enabling users to save and retrieve their preferred DataCards.
Utilized localStorage to persist bookmarks across sessions, ensuring user preferences were retained.
Implemented window event handlers to monitor and update bookmark states dynamically.
Visualization and CSV Handling:

Developed interactive data visualizations using Recharts, allowing users to explore datasets through charts like bar graphs, line charts, and pie charts.
Integrated CSV file readers, enabling users to upload external datasets and view them directly in the portal. This functionality made the system highly extensible and user-driven.
Static Pages and Embedding External Content:

Created static pages, such as the report page where users would be able to generate their reports made by tools in the website and uploading those reports for the community to see. 
Embedded external content using iFrames, allowing integration of third-party pdf readers into the portal where user can then view each others report in a pdf format.
Lessons Learned and Skills Acquired:
Through this project, I developed a deeper understanding of database management and how to design scalable systems for dynamic content rendering. Working extensively with React hooks improved my ability to manage state and lifecycle events efficiently. Implementing features like localStorage and event handlers enhanced my knowledge of web browser capabilities and user experience optimization.

The project also strengthened my skills in data visualization and user interface design, particularly through the use of tools like Recharts. Building a CSV file reader allowed me to learn more about file parsing and real-time data handling. Additionally, creating static pages and embedding iFrames taught me the importance of combining dynamic and static elements in a cohesive user interface.

Learn more at [HEX Repository](https://github.com/HACC2024/HEX).
