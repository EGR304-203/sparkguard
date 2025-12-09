---
title: Team Software Design
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


## Version 2.0

From the lessons we learned about the project and our individual components, a Version 2.0 would place much stronger emphasis on customer-facing features and meeting requirements from the outset. In the first iteration, we spent too much time in the design ideation stage under the assumption that our primary goal was to create a fully functional, polished product. In reality, our focus should have been on ensuring that our design fulfilled the customer’s requirements first, and then determining how to build something viable and useful within those constraints.

For Version 2.0, Armando’s current-sensing subsystem would concentrate on completing the postponed calculations—kilowatt-hour measurement, conversion to amperes, and instantaneous power in watts. These improvements are essential for achieving the stretch goal of a functional seven-segment display that provides meaningful energy-usage information to the user. Additional programming would be required to properly drive and update the display.

For Ayush’s subsystem, a major improvement would be selecting a geared motor or a bi-directional linear actuator, since the unit used in Version 1.0 did not meet the requirements imposed by our client. If that requirement were relaxed, the existing actuator design would still be suitable for controlling a locking door mechanism for the smart outlet.

For Manny’s subsystem, Version 2.0 should prioritize reducing the overall PCB size to better fit inside the outlet enclosure. The current design includes numerous jumpers and test points to support troubleshooting and to maintain flexibility in the event of part delays, but many of these could be consolidated or removed to simplify routing and reduce board area. Eliminating the audio gate entirely—which was ultimately unnecessary—would further decrease the footprint of the design.

Across all PCBs, Version 2.0 would also address component-to-connector clearance issues, particularly around the micro-USB ports used for programming the PIC microcontrollers. Both Armando’s and Manny’s boards experienced interference problems that made it difficult to load firmware, and ensuring proper spacing in the next revision would significantly improve usability and manufacturability.

## External links
1. [Link to Lucid Chart Diagram Source (Figure 1)](https://lucid.app/lucidspark/50a3b367-512a-4085-a351-7ba08a005a17/edit?viewport_loc=-1504%2C4113%2C4121%2C2114%2C0_0&invitationId=inv_718e862a-cc1e-4b68-8ead-81b798ccf1a2)

## References
[1] [Activity Diagrams - Unified Modeling Language (UML)](https://www.geeksforgeeks.org/system-design/unified-modeling-language-uml-activity-diagrams/)<br>
[2] [What is the difference between State Machine Diagram and Activity Diagram?](https://www.geeksforgeeks.org/system-design/what-is-the-difference-between-state-machine-diagram-and-activity-diagram/)