---
title: "Control Loop"
date: 2023-07-31T20:38:16+10:00
draft: false
---

```python
while True:
    # Sense: What position are the joysticks pushed to?
    joy_y_axis = controller.axis1.position()
    joy_x_axis = controller.axis2.position()

    # Decide: Is the position value too small to care about?
    if abs(joy_y_axis) < 10:
        joy_y_axis = 0
    
    if abs(joy_x_axis) < 10:
        joy_x_axis = 0

    # Act: Arcade drive!
    left_percent = joy_y_axis + joy_x_axis/2
    right_percent = joy_y_axis - joy_x_axis/2
    motor_left.set_velocity(left_percent)
    motor_right.set_velocity(right_percent)

    # Explanation for pause...
    wait(1, MSEC)
    # Go back to beginning of while loop, repeat.
```

Experience/Tutorial ideas
- Controlling multiple things in a control loop
- Where is the control loop for autonomous period?
