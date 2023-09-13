# Amber + SolarEdge Export limiting
Solaredge export limit during low or negative Feed in Tarrif (FiT) 

This is a blueprint that automates the exporting of solarpower to the grid when using Amber as a power provider in Australia that offer real time enrgy market rates.
This means that duing periouds of high renewable energy generation that the price of the grid is negative. Meaning that you would "pay" to export power to the grid

https://viewer.diagrams.net/?tags=%7B%7D&highlight=0000ff&edit=_blank&layers=1&nav=1&title=house%20power.drawio#R7VvZcts2FP0azbQP8XATJT3azjqNJ2ntNstLByJBCTVIMCBoSf36YiO4gFpsi1KayYNt4hLruecuAOGRf52u31CQL29IDPHIc%2BL1yH858jzXncz4HyHZKMlsGijBgqJYV6oFt%2BhfqIWOlpYohkWrIiMEM5S3hRHJMhixlgxQSlbtagnB7VFzsICW4DYC2JZ%2BQjFbKul07NTytxAtltXIrqPfpKCqrAXFEsRk1RD5r0b%2BNSWEqad0fQ2xAK%2FCRbV7veWtmRiFGTukAf3jz8vL353r8uMd%2Ffv6r6%2BYOF9f6F4eAC71gt8IvXghSPORf5XNC%2FFHL4BtKlQoKbMYio4d%2Fnq1RAze5iASb1ecB1y2ZCnmJde0foCUwfXWubsGEU4lSFLI6IZXqRpUIGoWec5YlVe1TtxA11k29DHVMqBpsDBd10jxBw3WI4DzLODuIC4AF70BDK7AxsKM6z8Xj0u4BguScWBySBGfDaS19GMl8vbjmqA1rCzmSDj7%2FgE4e6fEeWLhCGNuoLpIKFsSDhvAr2rpVZuddZ33hOQaq38gYxuNHSgZaSML14h9bjx%2FEV1djHXp5Vr3LAubqpDx5X5uFhqtRLFuJkutdh8bTFDC%2BFI4L17MSAaV5DUS0Mn3ChSBxG5Fc%2BBISSO4A2BfO1VAF5DtqBf2E4dCDBh6aM%2BjjwW66UeC%2BAwN4cKwQ7hg3O5CzV%2B36nDJTOPp9PItM%2Ba%2Bb%2BT5rkL5SY9vSVlA3ul7AmLbC6xQioFUacExZ5qDznHsd2zZr2PZ77THfGc7zFcP9gePriBbYPi40cY9owWd0QDmzM%2B427wShlsMoeegR88dzTCK1Pr2Ol5KGOe8cOEvX8yOpbmgjaXr21iGp3S8oYXYu0yukG6NbISeJBkIZ%2FuD1OSUUE0HcCJ7H68A47roSTMGdTC%2BP21h7wc2Td1KH03wDZ%2BPjv7sZ4YwbIbgBoOE%2FmDcDf3BxWHB3%2BrKCkR2Vyq%2FGSyPqLarJ2bhHhJULK2Z%2BaXB2X0srYn5pcXLfpYekXA6Nu9NSaeD8NKfztpk6iZHh7LSn23xlafipHsWTp7UM57OCR7ISW8QTnrWNmn2VF%2FpB3u7GpqX9tnJDYnnJU%2F8nRsZ4vYdP1UJZ05JBItif9Y5B9H9QlL7Q8kwyo54ZBI6bTz9SU9G1HdkEg6VELnjnnz0R3cEg6ZIe63%2BZ4p0AC2n52ThY1KgY4aN4FAGPTdwPM9lHHA%2BwrtBeXHA8cgRnGow7bC15zTE7%2FGpg20yXfs45KdPPcHB9PEPnN2uH3yiQw0th3pad1otfScja21FGBQFiroHmU0%2BDr%2Fze3Ic3XOgXMmeG247B4vmW%2B5juWHF7e7R49DcsDPss7pzr%2BvOvTO7c6%2Fvu8%2F%2F3Xi8LSnEaYzHd49kPF7XeCYnNh47F%2FqQy889nmOfqHCjYG1eFIySe3hNsPgcUkXJhIfIjghgtBCfkCKuaBFfr4SJoQjgS%2F0iRXG89XNUm33HsNFw3IK9Zxvb9%2F1pOBO1d7FGDbax%2FjBqCDonPWdXQ2g7xu9z19bwwN7ZTq69QxOd5273tuzynbYRW77z4Ox20qahf2AGwyOmuPpkquWiQrF9wt6sPWG%2Fe4ltT9bdqc8f1AyOGxHOegnJuZi0dnuz3VbAC%2FamzVjG5FGWsW%2B3Jz8w20mSFOtq7nENLDyzfbkd%2B%2BqaxcH21cmI%2Fe5HpqGTHPvOQjPJcV7wn0%2BIRxyO9RKJk%2FmIZAlalBToWiSR78R1oOs78QuDVCgV8%2FiYQrlW9faWYECFZcgoJqcG8ApsRKcjL%2FxWiguwV7cQ1gXTFssrVLwARH%2FRkoOCsoV5Pa%2FuQHC9fisRhcUFf36XbZ%2F1hpRCCsRzAetJwnXOTVSMiFIkxWQkrzM5IBMzyEQxKbkVi88TDoh0f3IQPXh8YX%2B4CLFYz5y3CRfiqZnCSJDvLIyKTcFgWoOVwQc5ZiEQshbewETNFGW8uURNNUCJYpW%2Bcd1Y6hxGQN1UkytWoGSEdcZitISGKUYXcuEkM7V050gkUfoudlcXYmYgi6BRQwZhXEFd4W5mJ6Xj31YCiCXCfWtXGq4BKIiphMxdpQpG03FOVlIuB%2BCtFz1dc6NyPqip9g6alLJPexmcBWWjmQHNsKno06FGXhI%2BW8jZRSBnJa17krPuIdiPmgd7nUA%2F7rlbGPTd%2BHZ33WV8Xio8s3zmkgh%2BxkJziP%2FcZ7IsTU6Ul%2BBB6I40PSuhTQlH4HVtJqLyzabpDC7z3PBME3ku5GCODa8Yn7u0tcRUBZI5tMwyZRkkSVqMq2wAJMpG1NBFmclJS2chWCGWtqqnttQXW5sTKTgE2v2IZjEFuug0hkkoSbue4hcJxIO2AEwK%2BGtnEcoJZYSmQAaNlHOMSbeTNPqOSKoG7BtEucSGBa2ACkASVjH3wgwXo6IZYGpfUi2bl%2BoQ0lWtZ%2Fv6Hd7frRyJnhqFCaRUuhHTo8RT%2BsQCpTlGCYJFd33GqXGXy%2B0cmyVjyOrKTUI1HCMm5N7iADf4qMQyXMpgeqd89xWnfE5VCrMi9L6QNJD5QXNR39m%2FjZhzRrOZ7nEifVdFn%2FJxnhfrf%2BZReVr9L1H%2Bq%2F8A

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


      


