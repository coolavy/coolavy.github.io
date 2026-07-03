---
layout: single
title: "CAN Distribution Hub"
permalink: /projects/can-distribution-hub/
author_profile: true
---

# Objective
In FRC, CAN is typically wired through a daisy chain, which means you connect a motor to a motor to another motor and so on until you have covered every device. This leads to problems such as unseen broken wires, and even if one of the wires is broken you lose all connection with your motors and are basically hopeless. The goal of this project is to fix that. Similar to a Power Distrubition Hub, a CAN Distrubtion Hub host all the motors CAN wires at one spot, and combines with an ESP-32 to monitor data and send it back to the RIO/Systemcore.
