# *Line-follower*

This is the final project for the Introduction to Robotics course taken in the 3rd year at the Faculty of Mathematics and Computer Science, University of Bucharest.

Team name: **fetitele_powerpuff**
Team members: [Andreea](https://github.com/AndriciucAndreeaCristina), [Carina](https://github.com/SaicuCarina), [Corina](https://github.com/corinagherasim)

Out of the three tries on the final circuit, our line follower robot completed the circuit best in *19.65 seconds*.

---

## *Contents*  <a id="0"></a>
- [Technical Task.](#technical_task) :clipboard:
- [Components.](#components) :electric_plug: 
- [Pictures of the setup.](#setup_pics) :hammer_and_wrench:
- [Process explanation.](#process_explanation) :exploding_head:
- [Final Presentation](#final_presentation) :racing_car:

---

## *Technical Task.* :clipboard: <a id="technical_task"></a>
The task involved working with a robotics kit and utilizing provided starter code. Our objective was to construct the machine, integrate six QTR-8A sensors, and fine-tune the PID.

To successfully pass the exam, the line follower had to complete at least one lap within a reasonable time frame. The final grade was determined based on specific time thresholds, with the target being around 20 seconds (an average).

---

## *Components.* :electric_plug: <a id="components"></a>
1. Arduino Uno
2. Power source (LiPo battery)
3. Wheels (2)
4. QTR-8A reflectance sensor, along with screws
5. Ball caster
6. Chassis
7. Breadboard
8. L293D motor driver
9. DC motors (2)
10. wires, zip-ties, screws as needed
    
---

# *Pictures of the setup.* :hammer_and_wrench: <a id="setup_pics"></a>
![line-follower setup](https://github.com/AndriciucAndreeaCristina/Line-follower/assets/68044359/51bccf61-24bd-4692-a1a3-a46431b0362c)

---

## *Process explanation.* :exploding_head: <a id="process_explanation"></a> 
The program incorporates an automated calibration process executed during startup. This calibration adapts the robot to varying environmental conditions by utilizing data from QTRSensors. As the robot may encounter different color intensities or lighting conditions, this initialization ensures optimal sensor sensitivity and responsiveness. 

The core of the line-following functionality lies in the PID (Proportional, Integral, Derivative) algorithm. This algorithm continuously adjusts the motor speeds to keep the robot precisely following the line. The proportional term (kp) helps the robot respond to the immediate error, while the integral term (ki) accumulates past errors to eliminate steady-state discrepancies. The derivative term (kd) anticipates future trends, minimizing abrupt changes. The PID constants (kp, ki, kd) have been fine-tuned through repeated testing on a controlled circuit, ensuring a balance between responsiveness and stability. 

---

## *Video showing our line follower on the final presentation.* :racing_car: <a id="final_presentation"></a> 
You can find the first lap of the robot on the final circuit [here](https://youtu.be/MrI7-eyq_eg).

---
