---
layout: project
type: project
image: img/ICStudy-SB.jpg
title: "ICStudy"
date: 2024
published: true
labels:
  - NextJS
  - PostgreSQL
  - PrismaORM
  - AWS
summary: "Study Buddy Application for creating study sessions with classmates or other students"
---

## Study-Buddy Overview
Welcome to my study-buddy website, a platform designed to facilitate collaborative learning by connecting students for study sessions. Below, I detail my key contributions to this project, the skills I developed, and the lessons learned.

## Contributions
#### Dynamic Session Cards

I created dynamic session cards that users can easily create to organize study sessions. These cards display all the necessary details about each session, such as the topic, time, and participants.
User Interaction with Sessions

I implemented functionalities allowing users to join or leave study sessions seamlessly. This feature ensures flexibility and encourages active participation.
Users can also delete their sessions, giving them complete control over their created sessions.
Database Integration

Developed forms to update our PostgreSQL database, ensuring that session information is accurately stored and retrieved. These forms facilitate the creation and management of session cards.
Built user profile management forms allowing users to create and update their profiles, ensuring personalized user experiences.


#### AWS S3 for Image Uploading

Integrated AWS S3 for user image uploads, enhancing the personalization of user profiles. This process involved:
POST Requests: Handled the image upload via POST requests to the S3 bucket.
IAM Configuration: Set up IAM roles and policies to secure and manage access to the S3 bucket.
CORS Configuration: Configured CORS to enable secure cross-origin requests, ensuring that images can be uploaded from our web application without issues.
Bucket Configuration: Properly configured the S3 bucket to handle image storage and retrieval efficiently.


## What I Learned

Throughout this project, I gained valuable insights and enhanced my technical skills in several areas:

Database Relationships

Many-to-Many: Learned to effectively implement and manage many-to-many relationships, which are crucial for linking users with multiple study sessions.
Many-to-One: Understood the nuances of many-to-one relationships, particularly in organizing multiple sessions under a single user profile.
One-to-One: Explored one-to-one relationships to ensure each user profile is uniquely associated with its image upload.
Backend and Frontend Integration

Gained proficiency in integrating frontend forms with a backend database, ensuring smooth data flow and user interactions.
AWS Services

Acquired practical experience with AWS S3, IAM, and CORS configurations, enhancing my ability to manage cloud-based resources securely and efficiently.

## Conclusion
This project has been a significant endeavor in my journey as a computer science student, providing me with hands-on experience in web development, database management, and cloud services. For a detailed view of the project and to explore the source code, please visit my organization's <a href="https://github.com/thesoftwaredevelopers/TheSoftwareDevelopers">GitHub Repository</a>.

