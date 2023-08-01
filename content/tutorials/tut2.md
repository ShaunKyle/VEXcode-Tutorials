---
title: "Competition Periods"
date: 2023-07-29T18:56:48+10:00
draft: false
topics:
---

# Introduction

A VEX Robotics Competition match is 2 minutes long, split into two different time periods: Autonomous Period (15 seconds) and Driver Controlled Period (1 minute 45 seconds).

During the Autonomous Period, robots operate without any help from humans using pre-programmed commands and sensor inputs.

During the Driver Controlled Period, humans can operate their robots via remote control.

***How does the robot know when it is Autonomous or Driver Controlled Period?***

Learning outcomes (SOLO taxonomy is useful here):
1. Identify the main elements of the Competition Template.
2. Describe the purpose of using the elements in the Competition Template.
3. Apply the elements of the Competition Template to an existing robot program.
4. Extra? What is an Event? How does a callback function work? Can you make your own?

Tutorial should probably be spread across multiple pages?

# Level 1: Identify

Open example program.

{{< quiz 
    "What is the"
    "a"
    "b"
    "c"
>}}

Question that identifies the purpose of autonomous()

Question that identifies the purpose of driver()

Question that shows Competition(autonomous, driver) registers callback functions. The functions don't function on their own.

Question that shows that "pre_autonomous" is not part of the Competition thing. It's just a function that we can choose to call before registering the Competition functions.

# Level 2: Describe

{{< figure src="/vexcode-help-events.png" width=500 >}}

# Level 3: Apply