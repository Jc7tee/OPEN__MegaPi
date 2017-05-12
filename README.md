# OPEN__MegaPi

The objective is to study how the MegaPi's firmaware works from signal receiving to execution of actuators.
I chose controlling the encoder motor on port 3 as the scenario.
Currently what I found is that:
 
parseData() -> runModule() by case statement RUN which corresepond to value 2
