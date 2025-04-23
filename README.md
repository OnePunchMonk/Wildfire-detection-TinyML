# 🔥 Wildfire Detection using TinyML

A TinyML-powered wildfire detection system designed to run on microcontrollers. This project leverages Edge Impulse for machine learning model development and deployment, and Wokwi for simulation and testing in a virtual environment.

## 🚀 Overview

Wildfires are a growing concern globally, and early detection is crucial in mitigating their impact. This project presents a lightweight, efficient wildfire detection model that can be deployed on low-power edge devices like the Arduino Nano 33 BLE Sense. Using TinyML techniques, the model classifies environmental conditions to detect signs of wildfire threats in real-time.

## 🧠 Model Deployment

The machine learning model was trained and deployed using Edge Impulse, a powerful platform for developing embedded ML applications. The pipeline includes:

- **Data Collection**: Sensor data simulating wildfire conditions (e.g., temperature, humidity, smoke levels).
- **Signal Processing**: Pre-processing raw sensor values.
- **Model Training**: Lightweight neural network optimized for microcontrollers.
- **Deployment**: Model exported as C++ library and integrated into Arduino firmware.

- **Edge Impulse**: Deployment can be found [here](https://studio.edgeimpulse.com/public/614756/live/impulse/2/validation).
## 🧪 Simulation with Wokwi

We used Wokwi to simulate and test our system without physical hardware. Wokwi provides an accurate emulation environment for the Arduino Nano 33 BLE Sense, allowing us to verify sensor readings, model inference, and alert outputs in a virtual setup.

### 🔧 Features

- Real-time wildfire condition classification
- TinyML model optimized for microcontrollers
- Fully simulated in Wokwi
- Compatible with Arduino IDE

## 📁 Project Structure

```
Wildfire-detection-TinyML/
├── model/                  # Edge Impulse exported model files
├── wokwi/                  # Wokwi simulation setup (diagram.json, code)
├── src/                    # Arduino firmware using the deployed model
├── README.md               # Project documentation
```

## ⚙️ Requirements

- Edge Impulse account
- Arduino IDE
- Wokwi emulator (or physical board)
- Compatible MCU (e.g., Arduino Nano 33 BLE Sense)

## ▶️ Getting Started

1. **Clone this repo**:
   ```bash
   git clone https://github.com/OnePunchMonk/Wildfire-detection-TinyML.git
   ```

2. **Open the Wokwi simulation**:
   - Load `diagram.json` on [wokwi.com](https://wokwi.com/) to test the simulation.

3. **Deploy to real hardware** (optional):
   - Open `src/` in Arduino IDE.
   - Upload to a compatible board with Edge Impulse model included.

## 🛠 Technologies Used

- Edge Impulse
- Wokwi
- Arduino Nano 33 BLE Sense
- TinyML / C++
