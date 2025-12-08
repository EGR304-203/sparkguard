---
title: Ideation and Concept Generation
tags:
- tag1
- tag2
---
## Sparky Smart Power Solutions<br>
## Intro/overview<br>

The process of generating feature ideas from our requirements and customer feedback took two team meetings and inernal discussions with the team as we compiled lists, ranked the features, and ultimately sorted them to create three different product options. At the end our team came up with the following product offerings:

- **The Sparky Charging Hub:** a light duty charging sation with simple scheduling and timing options. Our low cost option.
- **The Pro Model:** an enhanced version of the sparky wiht a higher amperage raiting, user interactible screens and more safety features.
- **The Paragon Model:**  our fully equipped version that contains all of the features of the above offerings plus a battery backup system and more power outage protections.

Below is the process that we went through in order to come up with these features, we explain our reasoning as to why some were not included and our thought process when doing our revision changes from our first to second pass of our features.<br>


## Generating Ideas & Features<br>

Our brainstorming process took place over two videoconference meetings on Zoom, supplemented by several informal follow-up conversations. All team members participated in these sessions, and ideas were documented to ensure a shared record of contributions.

To collect ideas, we used Lucid’s brainstorming diagram tool, which allowed us to visually map, expand, and organize potential features. We drew heavily from the “Product Requirements” team assignment, where we had compiled requirements based on customer feedback and reviews of comparable products. These reviews provided an important external perspective on user needs and common challenges, which we combined with our team’s own requirements list and insights from brainstorming. Together, these sources gave us a pool of more than 100 possible features.<br><br>
![Brainstorming All](Brainstormingwhole.jpeg)<br><br>
Once we had compiled the initial list, we grouped features into categories to clarify their purpose and relationships. The groups included Control & Monitoring, Hardware Features, Power & Performance, Connectivity & Compatibility, User Interface & Experience, Reliability & Safety, Affordability & Sustainability, and Advanced Features. These categories reflected different dimensions of the product’s functionality, usability, and market positioning. For example, Control & Monitoring encompassed how users interact with the device and observe its status, while Hardware Features captured the physical and electrical build of the product. Similarly, categories like Reliability & Safety emphasized protections and standards, and Affordability & Sustainability reflected both cost and environmental considerations.<br>

After grouping, we applied a ranking process to evaluate which ideas were most essential to the core goals of the project. By ordering features from most to least critical, we identified a set of “Core Features” that would form the foundation of the base product model. Additional features were then layered on to define more advanced product variations. This ranking exercise allowed us to balance innovation and user comfort with practical considerations such as feasibility and cost. The structured approach ensured that our design process emphasized both creativity and pragmatism, while giving us flexibility to differentiate across product tiers.<br>

Through this process of meeting, documenting, grouping, and ranking, we transformed an unstructured list of ideas into an organized and prioritized set of features. The outcome provided a clear roadmap for our design iterations and ensured that our product concepts remained aligned with both user needs and project goals. Ultimately, the brainstorming sessions gave us a strong foundation for moving forward into prototyping and refinement.<br>


## Brainstorming Participants, Tools Used, Resources, Grouping, & Ranking<br>

- ### Our brainstorming ideas grouped into categories that we created in order to place similar or related features in buckets to keep them organized. Below is a chart which is where our brainstorming began to shape our features into organized containers<br>
![Brainstorming ideas and categories](Brainstorming1.jpeg)<br><br><br><br>

- ### The brainstorming ideas were then ranked first into four tiers, High Importance Features (High tier), Important Features (Mid tier), Low Importance Features (Low tier), and the very low tier. Here we focused on keeping the features that would impact the cutomer the most for performance, safety, and reliability, while also making sure we to not neglet the main complaints that were brought up when we investigated customer feedback.<br>

- ### You will also notice our team quickly realized that we could group all these important and not so important features toghether. This is where we did our first official pass of our feature list, and is where we evolved our tier ranking system into some thing more practical. In this pass, we moved all critical features into our "Core features" container, then the more useful, but not critical features were placed in the "Added Features" container, and lastly the features that did not fall into the first two containers were placed in the "Cosmetic.." container.<br>
![Brainstorming ideas first pass](Brainstorming2.jpeg)<br>

- ### In our final pass the brainstorming ideas got re-ranked and with more stipulations such as feasability and budget contraints. Removed features are placed in the discarded features boxes.It is also important to note that the containers themselves were re-ordered to have the most important features on the left and least important features on the right.<br>
![Brainstorming ideas last pass and discarded ideas](Brainstorming3.jpeg)<br>
## Our 3 Concept Designs<br>

- ### The Sparky Charging Hub<br><br>
### Our base standard for greatness. A smart little charging hub that provides convenience and performance in a smaller package.<br>

![Base model sparky charging hub](basemodelsparky.png)<br>**Sparky Charging Hub model figure 1**<br> <br><br><br>

- ### The Pro Model<br><br>
### Equipped with extra features that bring comfort and more capabiltity to the end user.<br><br>
![Pro Model 1](pro1.png)<br>**Pro model figure 1**<br> <br><br><br>
![Pro Model 2](pro2.png)<br>**Pro model figure 2**<br> <br><br><br>
![Pro Model 3](pro3.png)<br>**Pro model figure 3**<br> <br><br><br>
- ### The Paragon Model<br><br>
### The top offering that we provide it has everything the Pro and Sparky have and more.<br><br>
![Paragon 1](paragon1.png)<br>**Paragon model figure 1**<br> <br><br><br>
![Base model sparky charging hub](paragon2.png)<br>**Paragon model figure 2**<br> <br><br><br>
![Base model sparky charging hub](paragon3.png)<br>**Paragon model figure 3**<br> <br><br><br>

## Concept Sketches / Further Design iterations
### Singular outlet with actuator and door latch
![showcase](earlyconcept.jpg)<br>
**Figure 1:** Our first concept design that was created during our first brainstorming session.<br><br>
In this design we originally intended for the charging hub to be protected in an enclosure with a door. The door was to be actuated via a DC motor with limit switches controlling when to stop the motor from spining and a H bridge to reverse the direction. While the idea was good for fulfilling class requirements, it did not fulfill our user needs and added more complexity.

### Singular USB port with door latch
![showcase](revisedconcept.jpg)<br>
**Figure 2:** After many internal discussions, our team narrowed down the next evolution of our concept to a feasable and attainable goal.<br><br>
We updated our original vision to simplify the operation of the door with a push/pull solenoid and a manually operated cover. As you notice in the design, the charging hub changed to a single USB port. We felt that creating a proof of concept for one USB charging port would better fall within the scope of the class project, while still fulfilling user needs.

**Justification:**<br>
While a microphone operated locking mechanism was not a main emphasis of the original user requirements, it fulfills [requirement 1.2](04-Product-Requirements.md#aspects) for weather protection, as well as an added implicit need for safety and security.


## Reflection
Because of rescoping our design to fulfill class requirements and limited budget/time, we reduced our initial plan of making a power strip to a single USB port with a microphone activated locking mechanism.

At the end of our project when we physically built the circuits to verify functionality, we realized that the pull solenoid we purchased was not bidirectional, meaning it could not be actuated in both directions. This meant we couldn't verify that a solenoid will move forward and backward, but a motor can when connected to the same circuit.

We also realized that solenoids that are truly bidirectional, without a permanent magnet or spring to do the opposite motion of the coil, are used in industrial applications such as [this one featured on Kendrion, a Dutch industrial actuator/controls company](https://www.kendrion.com/en/products-services/solenoids-actuators/linear-solenoids/reversible-linear-solenoids).