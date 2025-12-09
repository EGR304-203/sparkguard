---
title: Software Design
tags:
- tag1
- tag2
---

## Introduction
In this UML format diagram we walk you though each action that is taken when the user interacts with our product and how those trigger certain operations in our individual subsystems. The diagram is divided into a "User Side", "Voice Recognition", "Door Actuator", and "Power Monitoring" sections that showcase what operations happen when conditions are met.
Our current software proposal meets our requirements of localized control, voice recognition, reliable energy monitoring, and it provides safety features for the end user and their families.

## Research Questions
1. Does our subsystem logic have an end?
2. What are the shapes for UML activity or state machine diagram?
3. What better represents our logic: activity diagram or state machine diagram?

## Software Diagram

<object data="https://egr304-203.github.io/sparkguard/Team203SoftwareBlockDiagram.pdf" type="application/pdf" width="700px" height="700px">
    <embed src="https://egr304-203.github.io/sparkguard/Team203SoftwareBlockDiagram.pdf">
        <p>This browser does not support PDFs. Please download the PDF to view it: <a href="https://egr304-203.github.io/sparkguard/Team203SoftwareBlockDiagram.pdf">Download PDF</a>.</p>
    </embed>
</object>
**Figure 1:** This is our finalized software diagram. It has been updated to reflect our proven prototype features that we developed during testing, and any errors found during this period have been removed from our design.<br><br>


## Results (answers to research questions) 
1. Our logic does not have an end as it loops continuously as long as the design is being powered.
2. We successfully represented the logic with the correct shapes [1].
3. We decided an activity diagram best models our logic because our code will be instructions carried out one after another with only a few conditions that change the flow of operations, whereas a state machine model would mean each action has a condition before it [2].

## External links
1. [Link to Lucid Chart Diagram Source (Figure 1)](https://lucid.app/lucidspark/50a3b367-512a-4085-a351-7ba08a005a17/edit?viewport_loc=-1504%2C4113%2C4121%2C2114%2C0_0&invitationId=inv_718e862a-cc1e-4b68-8ead-81b798ccf1a2)

## References
[1] [Activity Diagrams - Unified Modeling Language (UML)](https://www.geeksforgeeks.org/system-design/unified-modeling-language-uml-activity-diagrams/)<br>
[2] [What is the difference between State Machine Diagram and Activity Diagram?](https://www.geeksforgeeks.org/system-design/what-is-the-difference-between-state-machine-diagram-and-activity-diagram/)