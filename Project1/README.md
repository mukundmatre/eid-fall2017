# ECEN 5053 Embedded Interface Design

# Project 1

## Author: Mukund Madhusudan Atre

**Project Description:**
>Setup Raspberry Pi 3 Board with latest Raspbian OS and Interface it with DHT22 Temperature and Humidity Sensor.
>The operation of Raspberry Pi was done with VNC Viewer which operates decently upto 1280x720 resolution on Wifi.
>A GUI is designed to systematically view the data obtained from sensor and build some additional features on top of it.


**Requirements for the Project**
>Raspberry Pi 3 with the latest Raspbian OS version flashed into the SD card.
> PyQt5 along with all supported libraries should be installed. This is assuming there is Python 3 already on the system (which was in the case of Raspbian OS)
>Install Qt Tools and Qt Creator on your laptop or desktop, it can also be installed on RPI3 but it will be really slow.
>Install UI to Python compiler library (pyuic5). This will give you your GUI written in PyQt5(Python) when you run this command:-
*pyuic5 -x gui_filename.ui -o python_filename.py*
>Where gui_filename.ui is obtained from QT creator and python_filename.py is the output file
>Connections should be made for DHT22 sensor as below:
> Vcc to Pin1; Data to Pin7(GPIO4); GND to Pin6


**Instructions for Running the Project**
>On Bash type: sudo python3 sensors.py
> A GUI will open displaying values for Temperature and Humidity
>For getting updated values, click on Reset Button
>For getting a graph for Humidity and Temperature variation against the number of readings, click on Plot Graph button.
>For setting the Threshold value of Alarm, input the values for temperature and humidity in the text boxes in front of Threshold label
>If the current reading passes the threshold provided in the text box, the level bar to the right will turn red in color.

**Features: Extra-Credits**
>A message space at the right bottom of the GUI Window shows messages about the status of data coming from the sensor. If the sensor is not detected or data is nor received somehow, it shows an error message.
>Display current data and time for every data reception.
>Display the current average of sensor data for temperature and humidity.
>Alarm activation for humidity and temperature values based on the thresholds provided by the user.
>Generation of graphs-plots for the obtained data from the sensor.
>The data obtained is stored in .csv file.

**References**
1. Qt Documentation
2. Stack Overflow
3. zetcode.com
4. References mentioned in the code
