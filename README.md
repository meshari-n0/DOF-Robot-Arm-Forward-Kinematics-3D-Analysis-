# DOF-Robot-Arm-Forward-Kinematics-3D-Analysis
This project presents the mathematical modeling and numerical analysis of a 3-DOF robotic arm using Forward Kinematics.

![WhatsApp Image 2026-02-19 at 6 39 11 AM](https://github.com/user-attachments/assets/d275cc62-f7a9-40a7-9045-c23605b9fc11)
# Forward Kinematics – 3 DOF Robot Arm (3D)

## Link Lengths
L1 = 15 cm
L2 = 10 cm
L3 = 4 cm

## Assumed Joint Angles
θ1 = 45°
θ2 = 65°
θ3 = -70°

---

## Forward Kinematics Equations

x = L1*cos(θ1)
  + L2*cos(θ1 + θ2)
  + L3*cos(θ1 + θ2 + θ3)

y = L1*sin(θ1)
  + L2*sin(θ1 + θ2)
  + L3*sin(θ1 + θ2 + θ3)

z = L1
  + L2*sin(θ2)
  + L3*sin(θ2 + θ3)

φ = θ1 + θ2 + θ3

---

## Numerical Calculation

# Link 1
x1 = 15*cos(45°) = 10.61
y1 = 15*sin(45°) = 10.61

# Link 2
x2 = 10*cos(45° + 65°)
x2 = 10*cos(110°) = -3.42

y2 = 10*sin(110°) = 9.40

# Link 3
x3 = 4*cos(45° + 65° - 70°)
x3 = 4*cos(40°) = 3.1

y3 = 4*sin(40°) = 2.6

---

## Final End Effector Position

x = 10.61 - 3.42 + 3.1 = 10.29 cm
y = 10.61 + 9.4 + 2.6 = 22.61 cm

z = 15 + 10*sin(65°) + 4*sin(65° - 70°)
z = 15 + 9.06 - 0.35
z ≈ 23.71 cm

φ = 45° + 65° - 70° = 40°

---

## Final Result

x ≈ 10.29 cm  
y ≈ 22.61 cm  
z ≈ 23.71 cm  
orientation φ = 40°
