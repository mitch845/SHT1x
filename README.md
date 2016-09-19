Libreria sht1x

uso:

    #include <SHT1x.h>
    #define dataPin 10
    #define clockPin 11
    SHT1x sht1x(dataPin, clockPin);

### readTemperatureC() ###

Returns a float within the valid range of the sensor of -40 to +123.8C.
A value of -40 is returned in the event of a communication error with
the sensor.

Example:

    float tempC = sht1x.readTemperatureC();

### readTemperatureF() ###

Returns a float within the valid range of the sensor of -40 to +254.9F.
A value of -40 is returned in the event of a communication error with
the sensor.

Example:

    float tempF = sht1x.readTemperatureF();

### readHumidity() ###

Returns a float within the valid range of the sensor of 0 to 100%.
A negative value is returned in the event of a communication error with
the sensor.

Example:

    float humidity = sht1x.readHumidity();
