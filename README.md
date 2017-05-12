# OPEN__MegaPi

The objective is to study how the MegaPi's firmaware works from signal receiving to execution of actuators.
I chose controlling the encoder motor on port 3 as the scenario.
Currently what I found is that:
 
runSerial() enable the bluetooth port. parseData() -> runModule() by case statement RUN which corresepond to value 2. runModule will choose the encoder by case statement ENCODER_BOARD which correspond to value 61. This is possible as the device type is pass through runModule in parseData
