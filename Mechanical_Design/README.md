# Mechanical Design Documentation

# Body and Chassis Design

The robot consists of a rectangular chassis with rounded edges to reduce sharp corners and provide a streamlined appearance. Aluminum is proposed as the chassis material because of its lightweight properties and durability. A small display is located at the front of the robot for facial expressions, while the battery and control unit are intended to be positioned near the center of the chassis to improve balance and maintain the center of gravity.

---

# Leg Design

The robot uses four identical legs. Each leg consists of an upper section and a lower section connected through a Hip Joint and a Knee Joint. This configuration simplifies the mechanical structure while maintaining adequate stability for quadruped locomotion.

---

# Degrees of Freedom (DOF)

Each leg includes two rotational joints:

- Hip Joint (1 DOF)
- Knee Joint (1 DOF)

Total Degrees of Freedom:

**8 DOF**

---

# Motor Selection

Servo motors are proposed for both the Hip Joint and the Knee Joint due to their precise position control and ease of implementation. A gearbox may be added if additional torque is required, although this would reduce movement speed.

---

# Preliminary Torque Calculation

Torque is calculated using:

τ = F × r

Where:

- τ = Torque (N·m)
- F = Force (N)
- r = Distance from the joint (m)

Force:

F = m × g

Example:

m = 0.5 kg

g = 9.81 m/s²

F = 4.9 N

r = 0.10 m

τ = 0.49 N·m

Therefore, the selected actuator should provide a torque greater than **0.49 N·m** with an appropriate safety margin.

---

# Stability and Center of Gravity

The proposed design places heavy components such as the battery and controller close to the center of the chassis to improve stability and minimize the risk of tipping during operation.

---

# Proposed Walking Gait

The robot is intended to use a Crawl Gait because it offers high stability by keeping three legs in contact with the ground while only one leg moves at a time.

Suggested stepping sequence:

1. Front Right
2. Rear Left
3. Front Left
4. Rear Right

---

# Expected Mechanical Challenges

- Limited motor torque
- Joint friction
- Foot slippage on smooth surfaces
- Weight distribution
- Motor heating
- Battery consumption

---

# Software

- Autodesk Fusion 360

