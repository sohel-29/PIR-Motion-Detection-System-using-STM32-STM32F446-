# PIR-Motion-Detection-System-using-STM32-STM32F446-
This project demonstrates motion detection using a PIR (Passive Infrared) sensor with an STM32 microcontroller. When motion is detected, an LED and buzzer are activated.

The system continuously reads the sensor output and triggers alerts based on motion presence.

Hardware Components....

STM32F446RE 
PIR Sensor (HC-SR501)
LED
Buzzer 
Jumper wires
Breadboard

🔌 Pin Configuration....

Component	STM32 Pin
PIR OUT	PC0
LED	PC11
Buzzer	PC10


🔧 Circuit Connections....

PIR Sensor
VCC → 5V
GND → GND
OUT → PC0
LED
Anode (+) → PC11 (via 220Ω resistor)
Cathode (-) → GND
Buzzer
Positive → PC10
Negative → GND

🧠 Working Principle....

The PIR sensor detects infrared radiation changes caused by motion.

No motion → Output LOW → LED OFF, Buzzer OFF
Motion detected → Output HIGH → LED ON, Buzzer ON

The STM32 continuously polls the sensor input and controls outputs accordingly.

💻 Code Logic.....

Read GPIO pin (PC0)
If HIGH:
Turn ON LED and Buzzer
Else:
Turn OFF LED and Buzzer

🚀 How to Run...

Open project in STM32CubeIDE
Build and flash to STM32 board
Power the PIR sensor
Wait for calibration
Move in front of sensor to test

🧪 Expected Output...

Condition	LED	Buzzer
No motion	OFF	
Motion detected	ON

🧑‍💻 Author

Mohammed Sohel
