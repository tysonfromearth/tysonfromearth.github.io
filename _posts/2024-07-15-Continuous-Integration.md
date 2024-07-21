---
layout: post
title: "Continuous Integration"
date: 2024-07-15 11:30:00 -0000
categories: project-management
---

### by Tyson Bryant
### Spring Term 2024 at Oregon State Univesity
#### Previous Team Projects
During my time in the Computer Science Post-Baccalaureate program at Oregon State University, I have worked on four group projects including the present project dealing with continuous integration. The other three projects are: 
1. A database for collectible cards
2. A microservice project
3. A user interface for a budgeting application

For the microservices project both my partner and I were responsible for creating a program that uses a microservice as well as the microservice needed by the other’s program. I was responsible for user research and reporting as part of the budgeting application user interface project.

Notable difficulties arose while completing the card database and budgeting application projects. While working on the card database my team realized that we were just creating a reference database of the included cards instead of tracking individual cards. So, we added a feature allowing users to save decks comprised of cards to meet the specifications of the project. This oversight was due to a general lack of experience with databases which became apparent as we completed more of the course. The problem associated with my budgeting application project was that the delineation of responsibilities was not as even as we first predicted, leaving me with less work than my partner. As with my database project, I chock this problem up to a lack of experience, this time with user interface design leading to bad workload estimates.

#### Working With Continuous Integration
While I was excited to employ continuous integration in a project, I did have the sole concern at the beginning of the project that my work in another class, Operating Systems, would distract me from being able to contribute a fair amount. To address this concern, I communicated with my team early in the process to let them know that my time would be limited for one week during which I had to finish a make-or-break assignment in Operating Systems. My teammates’ support and understanding was heartwarming. 

My approach for submitting code for review was to use a test-driven development process and make pull requests after each new test passed. However, as we continued to work on the project, I noticed that my first pull request had not yet been reviewed and with the due date looming I had to press on and keep making commits. Combined with my teammates’ chosen approach to submit complete functions and test suites, we had a minimal number of pull requests and a respectable amount of code to review per pull request.

This project was my first group project that used automated linting and testing as well as peer review before merging work into the main branch, providing valuable experience that helped me grow as a developer. For example, I was able to learn about the behavior of pull requests in active branches that are still getting commits. I also realized that I can play a significant role in future teams by sharing my understanding of big-picture concepts, such as the importance of regular, incremental contributions in continuous integration workflows, to keep my team on track and avoid unnecessary stress down the line.

Near the end of the project, one of my teammates requested help with a test that was not passing. I was able to figure out that the function was correct and that the test was not passing due to discrepancies in the argument provided to the function and the expected outcome. Being that extra pair of eyes and explaining what I found instilled in me greater confidence in my mentoring abilities.

#### Lessons for the Future
The continuous integration workflow facilitates better software development by ensuring that the code is tidy and functional. Automatic linter use guarantees conformance to a style guide. The existence of a testing suite also ensures that the code behaves as expected. Furthermore, frequent code reviews by peers reduce the likelihood of accumulating technical debt and promote the development of the team’s skills, which is likely to benefit the team’s future software development whether on the same project or a different project. 

Mandatory code review strengthens the weak links in each developer’s code. Over time, if any team member knows an ideal way to do something, their reviews will strengthen any related weak habits in the code of team members who are not as familiar with that problem. Even if only one person knows the best way to approach something, a chain effect results when they correct the issue in another team members code because then two team members can identify and correct that kind of mistake when reviewing code. This process will continue until that mistake no longer shows up in any contributor’s code. 

I employed test-driven development to create most of my code. Test-driven development helps code to avoid any extraneous or repetitive parts because a test-driven developer codes directly from one specification to the next using the least amount of code possible. This means code is likely to be easier to read, as well. This method also forces developers to create a testing suite as they go, which is important when working on a shared code repository because it prevents defective code from showing up in the production version.