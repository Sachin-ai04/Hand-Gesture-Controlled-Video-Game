# Hand Gesture Game Controller (ESP32 + MPU-6050)

A wearable gesture controller that maps hand movements to game inputs using an MPU-6050 accelerometer/gyroscope and an ESP32 microcontroller.

## 🎥 Demo
https://www.linkedin.com/posts/sachin-kushwaha-74b011325_electronics-iot-esp32-activity-7436296950792060928-apqI?utm_source=social_share_send&utm_medium=android_app&rcm=ACoAAFIMq-sB0gRAdNXELOVNfxtqT5caFzbdd5o&utm_campaign=copy_link

## 🛠️ Hardware Used
* **Microcontroller:** ESP32 (DOIT DEVKIT V1)
* **Sensor:** MPU-6050 (6-axis Accelerometer & Gyroscope)
* **Display/Output:** [Mention if you used LEDs or if it's just Serial output]
* **Connectivity:** [USB / Bluetooth / WiFi]

## 🔌 Circuit Connections
| MPU-6050 Pin | ESP32 Pin |
|--------------|-----------|
| VCC          | 3.3V      |
| GND          | GND       |
| SDA          | GPIO 21   |
| SCL          | GPIO 22   |

*(Update the pin numbers above to match your actual wiring!)*

## 🚀 How It Works
1.  The MPU-6050 reads the **Pitch** and **Roll** of the hand.
2.  The ESP32 processes these values to determine the direction (Up, Down, Left, Right).
3.  The commands are sent via [Serial/Bluetooth] to the PC to control the game character.

## 📂 Installation
1.  Install the **Adafruit MPU6050** and **Adafruit Unified Sensor** libraries in Arduino IDE.
2.  Connect the hardware as per the table above.
3.  Upload `main.ino` to the ESP32.
4.  Open the Serial Monitor (Baud Rate: 115200) to see the output.
