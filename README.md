# Komodo Energy Coding Challenge

## Problem
The challenge is to interrogate a sample of home energy data with different usage patterns. The intention is to investigate the feasibility of shifting loads to gain revenue from agile tariffs and demand side response signals. 
This is built upon in the second section, where a flexible load is simulated and the optimum schedue is calculated, based on both cost and convenience factors.  

## Setup
python==3.11.5
numpy==1.24.3
pandas==2.0.3
matplotlib==3.7.2


## Key assumptions
* Assume usage patterns are on same day as the tariff so we can apply them directly
* Assume flexibility payment is in pounds
* Assume the home with the heat pump has exactly the same home consumption as the heat pump + battery household
* Assume the standard tariff is the current Ofgem electric tariff  (ignore standing charge) https://www.ofgem.gov.uk/energy-price-cap
* For the simulator, assume that we know the tariff and device schedule a day ahead
* No AI used


## Future work on the load shifting simulator
* Convert the simple loop in the simulation to an optimiser. This would speed up the calculations, expecially important if there is more data. However the simple loop was good for prototyping as it is useful for debugging and understanding the results.
* There's a int/float bug that means that you cant specify a non-int power. Fix this.
* Investigate different tariffs. The tariff provided is for a weekday, try other days and times of year.
* Add functionality for injecting turn down/up events 
* Add the ability to specify more devices to shift and find the optimum schedule
* Add an inconvenience factor for during the day if the household is not at home



