# Amber + SolarEdge Export limiting
Solaredge export limit during low or negative Feed in Tarrif (FiT) 

This is a blueprint that automates the exporting of solarpower to the grid when using Amber as a power provider in Australia that offer real time enrgy market rates.
This means that duing periouds of high renewable energy generation that the price of the grid is negative. Meaning that you would "pay" to export power to the grid

# CT Clamp configurations an implications 

Due to the nature of the 2 systems of Tesla and SolarEdge you are able to configure them in diffrent ways. 

![Screenshot 2023-09-13 at 5 21 12 pm](https://github.com/Ralphy140/Amber/assets/85327073/8f02e8af-f7f9-443d-837d-5acb1965b78b)


Option 1 - With this configuration of the CT Clam placement the SolarEdge will always "See" the load that charging the battery requires. In this configuration you can set the export limit to 0 and no further action is required. 
Option 2 - The SolarEdge system will never see the battery charging and instead see if as grid export because it can not see the true value that is on the grid interconnect. In this instance you need to limit export to 5Kw while the battery is charging so the inverter will export power to chage the battery, Once the battery is full you need to reduce the value to 0 as the battery can no longer capture the power. 

how do i know if i have option 1 or option 2? In the MySolarEdge App you will be able to tell. If you are running off battery power after the sun has gone down the house will be showing as drawing 0 power from the grid (or very close). If you see normal amounts of power coming from the grid and the powerwall app shows you discharging to the house then you have option 2

Option 1 is the preferred option as it simplifies the grid export control and lets the SolarEdge inverter look after the calculations. This Blueprint works with Option 1 

This automation is based on several items 
# 1) SolarEdge HD Wave with consumption monitoring 
You will need to ensure that your solar system has the consumtion monitor option. This is so that the solar system knows how much power to 
generate to match your housees power demand. 
# 2) Amber as your power provider 
This is required to take advantage of the veriable rate that is on offer in the energy market leading to periods of low prices and also high prices 
# 3) Home assistant 
This is the software brain that is required to being the information to gether and drive action when conditions are met 
# 4) SolarEdge Modbus add on for Home assistant  - https://github.com/binsentsu/home-assistant-solaredge-modbus
This is the interface between home assistant and the SolarEdge inverter. This specific add-on is required as it privuides local control over your inverter 
It is critical that you have this module running before installing this blueprint as it will not be able to make any changes at all without it. 
The instructions on how to get this working are in the link above. you will know its off an running when you are able to see the details of your inverter in the 
Home assistant device and service page.
# 5) Amber integration for home assistant - https://www.home-assistant.io/integrations/amberelectric/
The Amber integration provides the pricing information about the grid to determin when you should be limiting production 
# 6) Import the  blueprint 
Once you have met all the above rewuirement import the blueprint with this link https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https://github.com/Ralphy140/Amber/blob/main/Export_Power_Limit_Blueprint.yaml


      


