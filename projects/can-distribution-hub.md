---
layout: single
title: "CAN Distribution Hub"
permalink: /projects/can-distribution-hub/
author_profile: true
---

In FRC, CAN is typically wired through a daisy chain, which means you connect a motor to a motor to another motor and so on until you have covered every device. This leads to problems such as unseen broken wires, and even if one of the wires is broken you lose all connection with your motors and are basically hopeless. The goal of this project is to fix that. Similar to a Power Distrubition Hub, a CAN Distrubtion Hub host all the motors CAN wires at one spot, and combines with an ESP-32 to monitor data and send it back to the RIO/Systemcore.

### 7/5/2026
I did some research and found out that FRC Team 118, the Robonauts, have done something very similar, except without an ESP-32. It's just a PCB that is daisy-chained on the inside which allows for all of the CAN wires to come to one place. It's very small and nicely well-thoughtout. Below is the Robonauts Can Node.

<img width="359" height="160" alt="Screenshot 2026-07-05 154238" src="https://github.com/user-attachments/assets/44db4d83-d175-4c3e-813b-b8aba5cf6882" />

### 7/17/2026
I've done more research and in theory come up with a decent solution with one slight issue: ISO11898-2 protocol recommends a maximum of 0.3 meters (roughly a foot) of wire for each component going into it for signal integrity. Most FRC teams use elevators or arms in pick-and-place games, which often extend upwards of 5-6 feet, clearly exceeding the maximum. To fix this problem, there are components called CAN repeaters, which basically take the signal and clean it up and then broadcast it so the signal is good. However, R716 states "Don’t alter the CAN bus. No device that interferes with, alters, or blocks communications among the roboRIO and the PCMs/PHs, and/or CAN motor controllers on the bus will be permitted." Because I have no idea if my idea if in violation of this rule, I have decided to get an answer from the FIRST Q&A.

<img width="593" height="201" alt="Screenshot 2026-07-16 140837" src="https://github.com/user-attachments/assets/665f6e53-f1c1-4205-9887-8687dd691258" />
