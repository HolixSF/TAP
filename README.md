# Thermo-Aggregation Project -- T.A.P.

[Project Link](http://thermo-aggregation-project.herokuapp.com/)

We built an open-source system to alert public health officials about communities that may be at high risk for flu and infectious disease outbreaks.  Using infrared non-contact thermometers affixed to Arduino devices in public places, we passively collect human temperatures and feed that data realtime to our servers. Our systems then identify communities with statistically significant amounts of abnormal temperature readings to notify authorities about communities with potential public health concerns.

In addition to promoting public health goals, we also make all of our code free and available for other Arduino enthusiasts.  This code is particularly useful for students who want to learn more about connecting Arduino devices to WiFi and APIs since there is limited documentation on this topic.  

## Details
Data is collected from infrared thermometer sensors built on Arduino Uno boards. One of the benefits of using an infrared thermometer is that it can collect temperature data quickly and without actually making contact with a person. This means that an Arduino device with an infrared thermometer sensor could be affixed to a building entrance and collect and transmit temperature data for every person that walked by it, providing hundreds of data points a day.
This application will work best when we have devices all over the country collecting and publishing information. Stay tuned for more information regarding how to build or acquire your own Arduino device and post data to our site! 

In order to contribute to this open source project, people can:
- upload data through their own Arduinos (instructions will be provided for this)
- or if they have no access to an Arduino and its sensor modules, people can also upload data with CSV files.


### How To Contribute Data
#### For People Who Want To Upload CSV Files:
The files must be formatted as .csv.  All temperatures are in Fahrenheit.

1. Once on the main map view, click on "Upload Data".
2. The data must be arranged in this sequence:
    ````
    [infrared-sensed-temperature],[humidity],[mq_2 (flammable gasses)]
    ````

    An example would be:
    ````
    85.0,0.8,75.0
    86.0,0.7,76.0
    87.0,0.9,78.0
    85.0,0.8,75.0
    86.0,0.7,76.0
    ````

#### For People Who Want To Upload Data Through Their Arduinos
##### Hardware:
The model of Arduino that we used was the Uno.  
These are the sensor modules that we have attached so far:
- **Adafruit_MLX90614** = the infrared & ambient temperature sensor
- **DHT** = the humidity sensor
- **MQ-2 Gas Sensor** = the flammable gasses sensor

You may use newer or better sensors than what was used here.

##### How To Program The Arduino:
The code that we used to program the Arduino is code that was modified from these:
- [Adafruit-MLX90614-Library (the infrared sensor)](https://github.com/adafruit/Adafruit-MLX90614-Library)
- [DHT-sensor-library (the humidity sensor)](https://github.com/adafruit/DHT-sensor-library)
- [DHT-sensor-library (the humidity sensor)](https://github.com/adafruit/DHT-sensor-library)

To see how we put it all together, here is our example:
- https://github.com/WALTERKERR/TAP/tree/development/Arduino

## Contributor List (In Alphabetical Order)
- Bernice Anne W. Chua
  - [GitHub](https://github.com/BerniceChua)
  - [LinkedIn](https://linkedin.com/in/bernicechua415)
  - [Twitter](https://twitter.com/ChuaBernice)
- Luis De Castro
  - [GitHub](https://github.com/HolixSF)
  - [LinkedIn](https://www.linkedin.com/in/holixsf)
- Michael Du
  - [GitHub](https://github.com/supermikol)
  - [LinkedIn](https://www.linkedin.com/in/michael-du-4927555)
- Jonathan Huang
  - [GitHub](https://github.com/jonwhuang)
  - [LinkedIn](https://www.linkedin.com/in/jonathan-huang-84659971)
- Walter Kerr
  - [GitHub](https://github.com/WALTERKERR)
  - [LinkedIn](https://www.linkedin.com/in/walter-kerr-2163336a)

(Credit goes to [Thomas Huang](https://www.linkedin.com/in/thomas-huang-155693103) for designing our logo.)

License
----

MIT
