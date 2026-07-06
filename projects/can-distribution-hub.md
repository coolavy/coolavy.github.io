---
layout: single
title: "CAN Distribution Hub"
permalink: /projects/can-distribution-hub/
author_profile: true
---

In FRC, CAN is typically wired through a daisy chain, which means you connect a motor to a motor to another motor and so on until you have covered every device. This leads to problems such as unseen broken wires, and even if one of the wires is broken you lose all connection with your motors and are basically hopeless. The goal of this project is to fix that. Similar to a Power Distrubition Hub, a CAN Distrubtion Hub host all the motors CAN wires at one spot, and combines with an ESP-32 to monitor data and send it back to the RIO/Systemcore.

### 7/5/2026
I did some research and found out that FRC Team 118, the Robonauts, have done something very similar, except without an ESP-32. It's just a PCB that is daisy-chained on the inside which allows for all of the CAN wires to come to one place. It's very small and nicely well-thoughtout.

<img width="359" height="160" alt="Screenshot 2026-07-05 154238" src="https://github.com/user-attachments/assets/44db4d83-d175-4c3e-813b-b8aba5cf6882" />

<small markdown="1">*Robonauts CAN Node*</small>
