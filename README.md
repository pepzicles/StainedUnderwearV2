# Stained Underwear
## Julia Daser and Pepi Ng

### About the project

This project aims to highlight the amount of time, resources and labour one spends coping with menstruation.

Our project sheds light on the often hidden and stigmatized inconveniences people face throughout their lifetime because of menstruation. We thus wish to proudly take ownership of our personal experiences with menstruation, and spark greater conversations around female reproductive health.

#### 1. Collecting the data
Pepi collected the number of times in which they scrubbed individual underwear stained with menstrual blood over the course of 11 days.

<img width="600px" alt="Screenshot 2023-11-18 at 8 56 01 PM" src="https://github.com/juliadaser/StainedUnderwear/assets/73170145/22bc6cb8-ad5f-41a4-b6df-617c0bb21348">

#### 2. Sending the Data
The amount of scrubs, and the time of day the underwear was scrubbed throughout those 11 days is stored in an API that is accessed from our hand-coded website. Using node.js, we connected our webpage to an Arduino that controls the physical robotic arm.

We followed this [tutorial by How to Mechantronics](https://howtomechatronics.com/tutorials/arduino/diy-arduino-robot-arm-with-smartphone-control/) to build the robotic arm.

We will be creating a web interface that shows a digital clock with the clock running in real time and the dates at which Pepi washed their underwear. The robotic arm will start scrubbing whenever it reached the time at which Pepi washed their underwear according to the data. The dates would be in real-time, to show the ongoing and never-ending labor that is expended on washing one’s stained, bloody underwear. The project will last 11 days- the number of days in which Pepi washed their underwear.

We will also be setting up a Raspberry Pi with a webcam camera that faces the robotic arm throughout these 11 days. The footage from the webcam camera will be live-streamed onto YouTube/ Twitch.

When the user clicks the first knob of the digital clock, the user is brought into an “about” page- essentially a description of the project. When the user clicks on the second knob of the digital clock, the user is brought into the livestream of the robotic arm via Twitch/ YouTube.
![Desktop - 2](https://github.com/juliadaser/StainedUnderwear/assets/73170145/455a9e08-8748-4822-b436-4d2e94ff7604)

<br>

**To link Arduino to the web interface, we will be using:**
Npm packages:

- npm express
- npm serialport

### To run the code:
- install dependencies
- In the terminal window in your code editor, type and enter: npm run develop


Link to our research paper: https://docs.google.com/document/d/1riK_md2-noeCT2EpTjOqRZSLSGz6CT_NuyUZCUM05jI/edit?usp=sharing

Updates:

20 Nov 23:
Successfully set up serial communication between Arduino and Web via node, npm express and nom serial port
Set up object containing data. The object will send data to the web interface and Arduino.
Successfully set up a web interface connected to Arduino and to show current time
Successfully triggered Arduino LED to turn on when it’s a certain time of the day
Successfully iterated through the day numbers once time reaches 12AM
