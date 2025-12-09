---
title: Block Diagram
tags:
- tag1
- tag2
---



## Introduction
The team block diagram demonstrates how each PIC Curiosity Nano micocontroller will take in analog signals, filter them, and process them through specific input pins, and which pins will output to analog devices or digital pins. Finally the diagram shows how we will communicate across microcontrollers using the 8 pin ribbon connectors. <br>
 
## Final Iteration
Below is our finalized team block diagram. The components listed reflect the parts we planned to use for our design, but due to ordering delays and sudden unexpected changes in manufacturing, some were not able to arrive on time and had to be changed for alternative parts. The alternative parts were similar components that we had on hand that worked to get our individual prototypes working.


<object data="https://egr304-203.github.io/sparkguard/Team203BlockDiagramFinal.pdf" type="application/pdf" width="700px" height="700px">
    <embed src="https://egr304-203.github.io/sparkguard/Team203BlockDiagramFinal.pdf">
        <p>This browser does not support PDFs. Please download the PDF to view it: <a href="https://egr304-203.github.io/sparkguard/Team203BlockDiagramFinal.pdf">Download PDF</a>.</p>
    </embed>
</object><br><br>

**Notes from this iteration:**<br>
1. All boards send/receive some sort of communication<br>
2. Functionality is simplified and aligns with updated design direction.<br>
3. Current sensor was added to meet power calculation requirements with a constant voltage.<br>
4. Updated microphone sensor path with individual diagram details<br>
5. Corrected format errors from previous diagram.<br>

### Team Connectors
![Team Connectors](TeamConnectorsFinal.png)

Attached [here](TeamConnectorsFinal.xlsx) is a link to the above excel sheet we developed with further details on the 8 pin connections between subsystems shown on our latest block diagram.

## Decision making process

**Meeting requirements and block diagram structure**<br>

We structured our block diagram to accurately show the inputs and outputs of our boards, which pins are being used, and what type of communication we are using between boards.

The result of this is three separate boards each with female 8 pin connectors that are all connected together. Connectors that only provide output or receive input signals are correspondingly labled with text.

The block diagram meets the product requirements because it features the new emphasized product features including: security/safety with the linear actuator solenoid, microphone, signal filtering and amplification where applicable, and the sensor usage with leds to show power being consumed. The fact that the entire device is independently controlled with these components means it is not reliant on external apps, eliminating connectivity issues, which was a highly requested feature during in our user needs section.

**Communication Structure**<br>

+ Subsystems<br>
Our communication protocol was simplified in order to meed the project deadlines and meet our project goals. As we investigated the options for communications between our boards and our individual components. For board to board communication and post filtering component communication we opted to use GPIO pins with digital signals and pull up or pull down resitors where appropiate. This was done to keep communication simple, especially when our boards talked to one another. The job of the pull up or pull down resitors was to not have a floating signal when an "OFF" or "ON" was desired.<br>

+ LEDS<br>
For debugging purposes we opted to use digital GPIO pins for our leds instead of PWM since we only needed to validate wheather a signal was "ON" or "OFF", or if a signal was in target or not. The dimming capabilities that we would have gotten via PWM was deemed unnecessary by our team. These LEDs inform the customer of basic information, such as power status, signal sent status, and signal received status. They are meant to inform the user that actions are taking place at a quick glance.<br>

+ UART<br>
In order to fullfill the requirement of showing our current sensor data for educating the customer and adding more calculations in furure iterations. We used UART1 with TX and RX pins in order to communicate the data that was being read by our microcontrollers to the end user. The current iteration displays this information via serial communication on USB, and we hope to change this to a display as planned to have this infomation more readily available for the customer. <br>


## Final Design Software Changes <br>

+ Armando Subsystem<br>
Due to time constraints, he had to cut down the stretch goal of having a current sensing with a seven segment display and programming it into his microcontroller. The original plan was to have this current sensor output on a seven segment display, but since time was running out and he needed to have some output of values to fullfill the client's requirements, he updated the code to only print out this value via a serial connection to show it was working.<br>

In the same avenue, some of his calculations that would have provided the customer with power usage data had to be kept simple. The kilowatt hour calculation, the conversion to show current in amperes, and showing instantaneous powere in watts had to be postponed for version two of the product since  we had to keep to the project deliverable deadlines.<br>

+ Ayush Subsystem<br>
Originally the idea was to have an incoming digital signal from Manny's board activate a linear actuator that was connected to an H-bridge. In order to fullfil our given requirements, he modified his code and circuit to send this digital signal to his microcontroller, so it could then send a digital signal to the H-bridge and the linear actuator to move it. Ayush had to add a closed and open pair of push buttons in order to independently test the functinality of the linear actuator for going in the forwards direction and going in the backwards direction which also had to be added on his code.<br>

+ Manny Subsystem<br>
On the first iteration, Manny was using a phototransistor in order to detect motion from a hand approaching it. Although, since our product will be used in a household, he changed it to a microphone with a push to talk button in order to restrict access to our power outlet and fullfill safety requirements. LEDs were also added to indicate what the status of the signal was in the loops.<br>

The last two major changes on Manny's subsystem was that the Goertzel logic was removed for a more simple threshold check for the cutt off frequency. Since I did not have time to continue experimenting with this amplitude analysis tool, going with a more simple option was more desirable to fullfill the deadline or the project while fullfilling our requirements.  This was a helpful detour as it helped Manny find out that the audio gate he had picked for controlling the push to talk function was not neccessary. Therefore the push to talk function was changed to work witht the same threshold instead of an additional hardware component. The hardware audio gate then was left on the design as an optional part.<br>
