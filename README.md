# 🎨 RGB Color Detection with TCS34725 & PSoC

This project demonstrates how to interface the **TCS34725 RGB color sensor** with a **PSoC 5LP microcontroller** over I2C, and visualize real-time RGB data using an LCD, USB UART terminal, and a custom **MATLAB GUI**.

> 📌 Developed as part of the *Embedded Systems Lab* at the **Indian Institute of Information Technology Guwahati**.

---

## 📍 Project Overview

* Read real-time RGB values from the TCS34725 color sensor
* Display values on:

  * 16x2 LCD display
  * USB UART terminal
  * Live MATLAB GUI plots and color display
* Detect dominant colors based on sensor data
* Visualize changes under different lighting conditions and colored objects

---

## 🛠 Apparatus Used

* PSoC 5LP Development Kit
* TCS34725 RGB Color Sensor Module
* 16x2 LCD Display
* USB cable & PC (for serial communication)
* Jumper wires & breadboard
* MATLAB (for GUI visualization)

---

## ⚙️ Features

*✅ I2C communication between PSoC and sensor
*✅ Real-time RGB reading and display
*✅ USB UART interface to send data to PC
*✅ MATLAB live plots of RGB channels
*✅ Visual color block updating dynamically in MATLAB
*✅ Clear and modular code in C (PSoC Creator) and MATLAB script

---

## 🧰 How It Works

1. Initialize I2C communication and configure the TCS34725 (integration time, gain)
2. Read raw RGB data continuously
3. Display RGB data on LCD
4. Transmit RGB data to PC via USB UART
5. MATLAB script reads and parses incoming data to:

   * Plot Red, Green, and Blue intensity graphs
   * Show a real-time color patch reflecting current RGB value

---

## 📦 Code Structure

```
├── PSoC_Firmware/
│   ├── main.c                # Main firmware (sensor init, read, display, UART transmit)
│   └── ...
├── MATLAB_GUI/
│   └── rgb_plot.m           # MATLAB script for plotting RGB data and visualizing color
└── README.md
```

---

## 🖥 MATLAB GUI Preview

<img src="https://via.placeholder.com/800x400.png?text=MATLAB+GUI+Live+Plots+and+Color+Block" alt="MATLAB GUI preview" />

> Live plots show real-time RGB intensity values; the color block updates dynamically.

---

## 📌 Results & Observations

* Successfully detected different colors (red, green, etc.) with stable readings
* Plots and color block changed consistently under different objects
* Dominant color detection logic functioned as expected
* Reliable communication over I2C and USB UART

---

## 🚀 Applications

* Color-based object sorting in robotics
* Ambient light detection and control
* Quality inspection in manufacturing
* Smart farming (analyzing plant health)
* Interactive installations and art

---

## 🧪 Future Work

* Integrate real-time data logging and plotting on PC dashboard
* Connect to IoT platforms for cloud-based color monitoring
* Add proximity sensing to improve accuracy
* Upgrade to full-spectrum sensors

---

## ✅ Conclusion

This project shows how a **TCS34725 color sensor** can be interfaced with a **PSoC** to read, process, and visualize real-world RGB data. It lays the groundwork for practical color-sensing applications in **robotics, IoT, and automation**.

---

## 📄 License

MIT License

---

