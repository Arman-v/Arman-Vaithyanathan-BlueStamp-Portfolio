# Ball Tracking Robot
This project is a ball tracking robot which uses OpenCV, a python library for computer vision to track and follow a red ball. This project uses many components including a Raspberry Pi, a PiCamera, 2 DC motors, a motor driver, a power bank, a simple chassis, and ultrasonic sensors. The robot will track the red ball using its PiCamera and find the most optimal path towards it. 

| **Engineer** | **School** | **Area of Interest** | **Grade** |
|:--:|:--:|:--:|:--:|
| Arman V | Lynbrook High School | Mechanical Engineering | Incoming Sophmore

![Headstone Image](ArmanV.jpeg)
  
<!---# Final Milestone-->

<!---**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**-->

<!---<iframe width="560" height="315" src="https://www.youtube.com/embed/F7M7imOVGug" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>-->

<!---For your final milestone, explain the outcome of your project. Key details to include are:
- What you've accomplished since your previous milestone
- What your biggest challenges and triumphs were at BSE
- A summary of key topics you learned about
- What you hope to learn in the future after everything you've learned at BSE-->



<!---# Second Milestone-->

<!---**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**-->

<!---<iframe width="560" height="315" src="https://www.youtube.com/embed/F7M7imOVGug" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>-->

<!---For your second milestone, explain what you've worked on since your previous milestone. You can highlight:
- Technical details of what you've accomplished and how they contribute to the final goal
- What has been surprising about the project so far
- Previous challenges you faced that you overcame
- What needs to be completed before your final milestone--> 

# First Milestone

<!---<iframe width="560" height="315" src="https://www.youtube.com/embed/F7M7imOVGug" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>-->

<!---For your first milestone, describe what your project is and how you plan to build it. You can include:
- An explanation about the different components of your project and how they will all integrate together
- Technical progress you've made so far
- Challenges you're facing and solving in your future milestones
- What your plan is to complete your project-->


### Key Components and Progress
For my starter Project I have chosen the Ball Tracking Robot as it is a challenging project which integrates two fields which I am very interested in: artificial intelligence and robotics. This robot is a simple chassis with two DC motors in the back and one castor wheel in the front and uses the python library OpenCV to track and follow a red ball. For my first milestone I have completed two things. First I setup the Raspberry Pi with my computer and displey its interface using the OBS software. I then connected the camera and was able to get it working so that its video is displayed. For the second part of this milestone I built and coded a working 3 wheeled chassis. For now the chassis moves forward, backward, and turns with keyboard input: buttons "w", "a", "s", and "d".

### Challenges 

Most of my challenges came on the software side of this milestone. My first roadblock came when I was imaging the micro SD card with the 64 bit OS. Due to my inexperience I fried the SD card and had to get a replacement setting me back a lot of time. I also had trouble setting up the PiCamera. It took me a lot of time to do the proper research and install the proper libraries and updates as well as learn the proper commands to get the camera to take pictures and display the video. My final obstacle came on the hardware side, and when everything was finished, the speed was a problem: the robot was driving way to fast. On the Raspberry Pi the digital pins only has two settings, LOW and HIGH and for the wheel this means on and off. Thus I had to learn how to use the Analog pin and code it as this can take a variety of values not just HIGH and LOW to change the speed at which the motor is spinning.

### Next Steps

Next, I have to use OpenCV and program the PiCamera to track the red ball by bounding it with a blue box. This is going to be extremely challenging and probably the most difficult part of the entire project. 

# Arduino Starter Kit Project

<!---**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**-->

<iframe width="560" height="315" src="https://www.youtube.com/embed/M5S7RC9FdJg?si=bSoDCnk9I-2Xry22" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
For my starter project I chose the Arduino Starter Kit as it is teaches the basics of C++ coding and circuitry and could be the basis for many mechanical engineering projects I choose to pursue in the future. I used the Arduino to build a simple circuit, that with the press of a button can turn on and off 2 seprate LED lights. When the button is pressed or read as HIGH the blue LED is set to LOW, or off, and the green LED is set to HIGH, or turns on, and vice versa when the button is read as LOW, or is not being pressed. I created this circuit using an Arduino, a proto shield, a handful of hook up wires, 3 resistors, a button, and a bread board for testing. 

### Challenges

Most of my challenges came from my inexperience with an Arduino and its accessories. It took me some time to learn how all the inputs and outputs work: motors, servos, LEDs, motion sensors, buttons, and switches. My first challenge came in choosing to use the motion sensor. I had wired everything correctly, but the sensor would pick up everything in such a large radius that the LED was getting too many signals at once. I had then changed to the button, but I faced an obstacle where one of the LEDs where not turning on. I then realized that two components - the button and the red LED - were on the same row of the breadboard causing a short, and when I fixed that the circuit was finally ready to move to the proto shield. My final challenge was moving the entire circuit. I did not have a lot of soldering experience and soldering so many small components caused me to melt many wire coverings and solder into unnecessary holes. The circuit was finicky and sometimes would not work, but I used a little more solder, made sure the connections between the wires were secure and tested connections with hook-up wires to finish the project.

### Takeaways

My main takeaways from this project were in building circuits and C++ programming, two very important skills for future projects. I learned how to build and test cuircuits on an Arduino with hook up wires and a breadboard, solder components to a protoshield and troubleshoot programming and wiring issues. I also learned how intiate inputs and outputs in C++, basic if and else statements and while loops(both things I had learned before).

<!---
# Schematics 
Here's where you'll put images of your schematics. [Tinkercad](https://www.tinkercad.com/blog/official-guide-to-tinkercad-circuits) and [Fritzing](https://fritzing.org/learning/) are both great resoruces to create professional schematic diagrams, though BSE recommends Tinkercad becuase it can be done easily and for free in the browser. -->

# Code

### Starter Project Code

```/*
  Button

  Turns on and off 2 LEDs connected to digital pin 13 and 12,
  when pressing a pushbutton attached to pin 2.

*/

// constants won't change. They're used here to set pin numbers:
const int buttonPin = 2;  // the number of the pushbutton pin
const int led13 = 13;    // the number of LED pin
const int led12 = 12; // the number of the LED pin 2
// variables will change:
int buttonState = 0;  // variable for reading the pushbutton status

void setup() {
  // initialize the LED pin as an output:
  pinMode(led13, OUTPUT);
  pinMode(led12, OUTPUT);
  // initialize the pushbutton pin as an input:
  pinMode(buttonPin, INPUT);
  Serial.begin(9600);
}

void loop() {
  // read the state of the pushbutton value:
  buttonState = digitalRead(buttonPin);

  // check if the pushbutton is pressed. If it is, the buttonState is HIGH:
  if (buttonState == HIGH) {
    // turn LEDs on and off:
    digitalWrite(led13, LOW);
    digitalWrite(led12, HIGH);
    Serial.println("On");
  } else {
    // vice versa:
    digitalWrite(led13, HIGH);
    digitalWrite(led12, LOW);
  }
}
```

<!--- 
# Bill of Materials
Here's where you'll list the parts in your project. To add more rows, just copy and paste the example rows below.
Don't forget to place the link of where to buy each component inside the quotation marks in the corresponding row after href =. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize this to your project needs.

| **Part** | **Note** | **Price** | **Link** |
|:--:|:--:|:--:|:--:|
<!---| Item Name | What the item is used for | $Price | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
| Item Name | What the item is used for | $Price | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
| Item Name | What the item is used for | $Price | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
-->

<!--
# Other Resources/Examples
One of the best parts about Github is that you can view how other people set up their own work. Here are some past BSE portfolios that are awesome examples. You can view how they set up their portfolio, and you can view their index.md files to understand how they implemented different portfolio components.
- [Example 1](https://trashytuber.github.io/YimingJiaBlueStamp/)
- [Example 2](https://sviatil0.github.io/Sviatoslav_BSE/)
- [Example 3](https://arneshkumar.github.io/arneshbluestamp/)

To watch the BSE tutorial on how to create a portfolio, click here.-->
