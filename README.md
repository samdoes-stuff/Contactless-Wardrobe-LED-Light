# Contactless-Wardrobe-LED-Light

This project uses a **Hall-effect sensor-based LED driver (APS13568)** to automatically control a wardrobe light. When the wardrobe door opens and the magnet moves away from the sensor, the light fades in. When the door is closed and the magnet is near, the light fades out. It provides a sleek, contactless solution with soft ON/OFF features.

## 🔧 Features
- Contactless LED control using an omnipolar Hall-effect switch.
- Fade-in/fade-out LED transitions.
- Soft start and soft off behavior.
- Over-temperature and short circuit protection.
- Configurable LED current (up to 150mA).
- Configurable magnetic polarity via POL pin.

## 📦 Bill of Materials (BOM)

| SR. | QNTY. | REF.   | DESCRIPTION           |
|-----|-------|--------|------------------------|
| 1   | 1     | CN1    | 5 PIN HEADER CONNECTOR |
| 2   | 1     | C1     | 1uF/16V SMD 0805       |
| 3   | 1     | C2     | 2.2uF SMD 0805         |
| 4   | 1     | D1     | WHITE LED              |
| 5   | 1     | R1     | 4K7 SMD 0805           |
| 6   | 2     | R2, R4 | 0E SMD 1206            |
| 7   | 1     | R3     | 1K SMD 0805            |
| 8   | 1     | U1     | APS13568 SMD SO8       |


### Schematic

![Screenshot 2025-05-21 223646](https://github.com/user-attachments/assets/1be24af0-0bf8-4865-be1d-a1c71f06f214)

### PCB Layout

![Screenshot 2025-05-21 222004](https://github.com/user-attachments/assets/be34cc20-5cfd-40d9-a263-0376fc439e0d)


### 3D View

https://drive.google.com/file/d/16dX2fbXP9qhfUznsYit0iP89W2JZGaH7/view?usp=sharing

### Gerber File

https://drive.google.com/file/d/1-jYX_K-TRQFvpCvhlMdSA4oJoc6tLWQU/view?usp=sharing


The heart of the project is the **APS13568 IC**, which is an ultra-sensitive, omnipolar Hall-effect switch with an integrated linear LED driver. This IC simplifies wardrobe lighting by replacing mechanical switches with a reliable magnetic sensor.

When the door is **opened** (magnet is far), the LED **turns on smoothly**. When the door is **closed** (magnet is near), the LED **fades out**. Resistor `R3` sets the LED current (~100mA), and capacitor `C2` controls the fade duration. Optionally, removing resistor `R4` reverses the magnet logic.

Ideal for:
- Wardrobes
- Glove boxes
- Task lighting
- Automotive mirrors

---

## 📎 Notes
- Fade-in/fade-out adjustable via `C2`
- LED current adjustable up to 150mA
- Default polarity: **LED ON when magnet is far**


Peace!!!!

