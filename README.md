# Komodo Energy Coding Challenge

## Problem
The challenge is to interrogate some home energy data with different usage patterns, with the intention of investigating the feasbility of shifting loads to gain revenue from agile tariffs and demand side response signals. 
This is built upon in the second section, where a simulation of a flexible load is modelled and the optimum schedue is calculated, based on both cost and convenience factors.  

## Setup
python==3.11.5
numpy==1.24.3
pandas==2.0.3
matplotlib==3.7.2


## Key assumptions
Use agile tariff including VAT. This is what the homeowner will pay.
Times are UTC.
Usage patterns are on same day as tariff so we can apply them directly
Assume flexibility payment is in pounds
The home with the heat pump has exactly the same home consumption as the heat pump + battery
The standard tariff usef is the current Ofgem elec tariff  (ignore standing charge) https://www.ofgem.gov.uk/energy-price-cap
No AI used
It's worth it if it's not too inconvenient and the cost is >10p


## Future work
Optimiser?
Fix 0.5 kWh
This is for a weekday
Different tariffs
Different power/duration
Additional devices to shift
Inconvenience during the day (not at home)
Also gain money from turn down/up


