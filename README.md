# CS 350 – Emerging Systems Architectures and Technologies

## About This Portfolio

This repository contains two projects I worked on in CS 350 using a Raspberry Pi. Before thiecourse, I had programming experience, but getting software to work with physical components was a different challenge. I chose these projects because they show how I worked with hardware, wrote Python code to control it, and figured out what was going wrong when something didn't behave the way I expected.

## Artifact One: Raspberry Pi Thermostat

For my final project, I built a thermostat system that uses temperature readings to determine whether heating or cooling should be active. The Raspberry Pi communicates with the connected hardware, while the LCD displays information about the system. Buttons let the user change the settings, and LEDs indicate what the thermostat's doing. The state machine helps keep the behavior organized instead of having everything happen at once.

One part I think I did particularly well was testing the thermostat under different conditions instead of assuming it worked after the first successful run. I checked the heating and cooling behavior and watched how the LEDs responded. At one point, the LCD stopped updating even though other parts of the program were still running. That was frustrating because the display made it look like the entire system had frozen. Working through the problem taught me to check each part of the system separately before deciding where the issue was.

If I went back to improve the project, I'd spend more time separating the display updates from the thermostat logic. That'd make it easier to troubleshoot a display problem without having to work through the rest of the program. I would also add more testing around button presses and changes between heating and cooling states.

## Artifact Two: Milestone Three – Input With Buttons

My second artifact's the button-controlled Morse code project. This milestone used buttons to control messages and an LCD to show what the program was sending. The challenge was making sure the input triggered the correct behavior and that the system returned to the right state afterward.

I chose this one because I remember having a problem where the LCD stayed on "sending: SOS" even after I pressed the button. The program was responding, but the display was not behaving the way I wanted. I had to go back through the code, look at how the states changed, and test the button again. Once I fixed it, the system responded the way it was supposed to. That was one of the more useful lessons from the course because I could actually see how a small mistake in the program affected the hardware.

I think I did well at sticking with the testing until the button and display worked together. If I improved this project, I would make the state changes easier to follow in the code and add a clearer way to show when a message had finished sending.

## Tools, Resources, and Skills I Can Reuse

The biggest addition to my set of tools was getting comfortable working with a Raspberry Pi through SSH from my Mac. I used Terminal to connect to the Pi, transferred Python files between the two computers, and edited code in VS Code. I also used draw.io to plan out state machines. Having to work between my Mac and the Pi took some getting used to, but it gave me a better understanding of how to develop and test code on a separate device.

I can see myself using these skills again in other programming projects. State machines are especially useful when a program has several possible conditions but needs to behave predictably. I also got better at troubleshooting by changing one thing, running the program, and checking what actually happened rather than making a bunch of changes at once.

## Keeping the Projects Readable and Maintainable

I tried to keep the Python code organized around what each part of the system needed to do. Using separate functions and understandable names makes it easier to come back later and figure out how the program works. The state machine diagrams also help explain the logic without requiring someone to read every line of code first.

There is still room to improve both projects. If I continued developing them, I would make the hardware settings easier to change and add more comments around the parts of the code that handle transitions. I would also test more edge cases, especially repeated button presses. My goal would be for someone else to understand the projects and make changes without having to retrace every troubleshooting step I went through.

## Repository Files

- `Thermostat.py` – Final thermostat program
- `Milestone3.py` – Button-controlled Morse code program
- `README.md` – Project descriptions and reflection

The two Python files are the portfolio artifacts. Supporting state machine diagrams, photos, or demonstration videos can be added separately if needed.
