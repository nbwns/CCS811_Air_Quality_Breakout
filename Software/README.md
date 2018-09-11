SparkFun CCS811 Software
=================================

Example software for use with CCS811.

Python Example
==============

Python Example is tested on Raspberry Pi 3. It use *pigpio* library for i2c
 communication which is installed on the RPi by default. Before usage start the pigpio 
 library as a daemon.
 
 > sudo pigpiod
 
 Run example with

> python ccs811.py

It connects to AWS IoT, checks and publish the data every 5 sec. You can define your own AWS config in the `app.cfg` file and store the certificate, private key and root CA alongside the configuration file.