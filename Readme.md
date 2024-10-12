# Drive Pulse

## Description
**Drive Pulse** is an IoT-based health monitoring system designed to evaluate essential health metrics such as temperature, heart rate, alcohol levels, and air quality. It uses multiple sensors to collect data and presents the results on a TFT display. Additionally, it incorporates fingerprint recognition for user identification.

## Features
- **Fingerprint Recognition**: Identifies users through fingerprint authentication.
- **Heart Rate Monitoring**: Uses MAX30105 sensor to check heart rate and SpO2 levels.
- **Temperature Monitoring**: Measures body temperature with a DS18B20 sensor.
- **Alcohol Detection**: Detects alcohol levels using the MQ-3 sensor.
- **Air Quality Detection**: Uses MQ-3 and MP503 sensors to measure air quality.
- **CO2 Level Detection**: Monitors CO2 levels with the MH-Z19C sensor.
- **TFT Display Interface**: Displays results and guides users through each step.
- **Humidity Tracking**: Measures environmental humidity using a DHT22 sensor.

## Components
- **MAX30105**: Heart rate and SpO2 sensor
- **DS18B20**: Temperature sensor
- **MQ-3**: Alcohol sensor
- **MP503**: Air quality sensor
- **MH-Z19C**: CO2 sensor
- **DHT22**: Humidity sensor
- **Adafruit Fingerprint Sensor**: For user authentication
- **TFT Display**: For displaying information
- **ESP32 / Arduino**: Microcontroller

## How It Works
1. **Fingerprint Authentication**: User places their thumb on the fingerprint sensor.
2. **Alcohol Detection**: If authenticated, the user blows air into the alcohol sensor.
3. **Temperature Measurement**: If alcohol level is within limits, temperature is measured.
4. **Air Quality and CO2 Monitoring**: Simultaneously, the device monitors environmental conditions.
5. **Heart Rate Check (Optional)**: Collects heart rate and SpO2 data if enabled.
6. **Display Results**: All metrics are shown on the TFT screen.

## Setup Instructions
1. Connect all sensors and components to the microcontroller as per the wiring diagram.
2. Install the required libraries:
   - `Adafruit Fingerprint Sensor`
   - `TFT_eSPI`
   - `MAX30105`
   - `DallasTemperature`
   - `DHT`
   - `MHZ`
3. Upload the code to the microcontroller.
4. Ensure the fingerprint templates are enrolled.
5. Power the device and follow the instructions on the TFT display.

## Libraries Required
- **Adafruit_Fingerprint**: For fingerprint recognition
- **TFT_eSPI**: For TFT display control
- **MAX30105**: For heart rate sensor
- **DallasTemperature**: For DS18B20 sensor
- **DHT**: For humidity sensor
- **MHZ**: For CO2 sensor

## Usage
- Place your finger on the fingerprint sensor to initiate the process.
- Follow the on-screen instructions to complete alcohol, temperature, and air quality checks.
- Monitor health data and air quality levels in real-time on the TFT display.


