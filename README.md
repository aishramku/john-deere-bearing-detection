# John Deere Baler Bearing Health Monitor

Society of Women Engineers x John Deere | Nov 2023 - May 2024

## The Problem

Round balers have bearings that keep the shafts spinning smoothly. When a bearing wears out, it heats up from friction, and since balers are full of dry hay, an overheated bearing can actually start a fire. A cracked bearing is also a major structural failure and dangerous for the farmer.

The catch is that bearings are really hard to keep an eye on, especially while the baler is running. The operator has no way of knowing a bearing is in trouble until it's too late.

John Deere wanted a way to catch this early.

## The Solution

A monitoring system that checks the bearing's temperature and vibration nonstop and alerts the operator in real time on a tablet in the cab.

The system sorts every reading into three levels:
- Safe: no action needed
- Within 10% of the danger limit: warning that it's getting close
- Out of range: alert that the bearing is in danger

It also had to work in any outdoor conditions, fit into John Deere's existing balers, and be cheap enough to mass produce.

## What I Did

I was on the product design side, which meant building the physical system that holds everything together.

- Designed the shaft in SolidWorks, which I learned from scratch for this project
- Drew and evaluated the shaft blueprints so the bearing would fit on it and the temperature and vibration sensors could sit inside, with wiring running through the shaft
- 3D printed the shaft and went through multiple versions, adjusting measurements each time until the bearing, sensors, and support all fit exactly
- Drew the blueprints for the wood support
- Cut and built the wood support and a custom base to hold the Arduino and breadboard
- Assembled the final prototype and added or removed parts to make the design work better
- Went on a site visit to John Deere's factory in Ottumwa, Iowa to see how balers are made and hear from their teams

## How the Full System Works

1. A hexagonal bore ball bearing sits on the 3D printed shaft
2. Temperature and vibration sensors inside the shaft read the bearing's condition
3. An Arduino UNO R4 collects the readings
4. A Python script sends the data to Firebase
5. An Android app on the tablet shows the bearing temperature and the alert level

## Challenges

- Getting exact measurements so the shaft fit the bearing, sensors, and wood support perfectly. This took several rounds of redesigning and reprinting.
- Learning SolidWorks, Arduino, wiring, and how the sensors work, all from zero

## Results

- Built a working prototype and demoed the app showing all three alert levels
- Spent only 15% of the budget ($556 in parts), which proved the system could be cheap to mass produce
- Presented the final prototype to John Deere

## Tools

SolidWorks, 3D printing, Arduino UNO R4, temperature and piezo vibration sensors, Python, Firebase, Android Studio
