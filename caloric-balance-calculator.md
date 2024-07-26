---
layout: page
title: "Caloric Balance Calculator"
permalink: /cbc
---
Created by Tyson Bryant and Hugh McBarron

Repository URL: [github.com/tysonfromearth/Caloric-Balance-Calculator](https://github.com/tysonfromearth/Caloric-Balance-Calculator)

Caloric Balance Calculator is a simple progam that demonstrates two important concepts in software engineering: microservices architecture and inclusivity heuristics.

## Microservice Architecture
 Microservice architecture splits the components of a program into separate applications, or microservices, that run in separate processes and could be useful independently from the main program. An advantage of implementing components as separate services is the ability to work on the microservice without disrupting other parts of the software. 

Caloric Balance Calculator is split up into a client-side user-interface and a server-side microservice. Communication between the two is handled with [PyZMQ](https://pyzmq.readthedocs.io/). The Caloric Balance Calculator's front end collects information from a user about how many calories they have consumed today and what their general level of activity is. The information is then sent to the PyZMQ pipeline and received by the microservice. The microservice uses the information to calculate the user's caloric balance and sends the result back to the PyZMQ pipeline. From there, the front end recieves the result and displays it to the user. 

![image](/assets/cbc-uml.png)
A UML sequence diagram showing the inter-process communication pipeline.

While I handled the user interface, my teammate Hugh imlemented the microservice. This arrangment provided an opportunity to practice coordination, communication, and project management in addition to the technical aspects of the project. 

## Inclusivity Heuristics: Abi, Pat, and Tim
Despite being a simple program, Caloric Balance Calculators incorporates the eight Cognitive Style Heuristics developed by researcher's as part of Oregon State University's [GenderMag Project](https://gendermag.org/). The concepty behinds these inclusivity heuristics is to ensure that a program is usable and useful to users with different levels of ability and attitudes, from power users that get a kick out of exploring advanced features to low-skill users that just want to get something done without getting overwhelmed or wasting time.

To facilitate this goal, developers keep three personas with different cognitive styles in mind when developing a user interface. Consideration of these personas is accomplished by following eight rules-of-thumb:

1. Explain the benefits of using new and existing features
2. Explain the costs of using new and existing features
3. Let users gather as much information as they want, and no more than they want
4. Keep familiar featurs available
5. Make undo/redo and backtracking available
6. Provide an explicit path through the task
7. Provide ways to try out different approaches
8. Encourage tinkerers to tinker mindfully

Caloric Balance Calulator includes an about feature explaining how to use the program (heuristic 1). The about feature's information is only displayed if the user chooses to display it (heuristic 3) and the selection screen tells the user about how long it takes to get the information about the program (heuristic 2). The information presented by the about feature provides instructions on how to use the calculate feature (heuristic 6) and users can access the about information by reading or listening (heuristic 7). User's can enter the familiar "z" instead of a number of calories to go back to the selection screen (heuristics 4 and 5). Finally, the flow of choices prevents invalid input and ultimately returns the user to the selection screen, providing the user with opportunity to try out different values without going too far off the beaten path (heuristic 8).

## Conclusion
Caloric Balance Calculator was an enlightening project that allowed me and Hugh to learn about microservices architecture, inclusivity heuristics, and project management as a team.
