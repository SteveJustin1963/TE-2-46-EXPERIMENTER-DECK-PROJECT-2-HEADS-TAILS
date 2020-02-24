# TE-2-46-EXPERIMENTER-DECK-HEADS-TAILS PROJECT TWO

![](https://github.com/SteveJustin1963/TE-2-46-HEADS-TAILS/blob/master/cct.png)

https://easyeda.com/editor#id=c2c46e31d9dc4d67b755dad756e01ee9

This project adds a further 9 parts to the HEE HAW SIREN to make our 2-LED readout "HEADS OR TAILS". You must complete the HEE HAW first and have it operating correctly before starting this project. This way you are testing your workmanship in stages...its no good completing a project to find it doesn't work.  

## THE ORIGIN OF HEADS OR TAILS 
In days gone by, players would toss a penny to see who would commence playing a game. This custom is still carried on in cricket. When pennies were in full circulation, one of the simplest games in the world used a penny as the sole betting medium. Although highly illegal, groups or sharp, daring punters would gather behind deserted buildings to play what they called "the fairest game in the world" ; TWO-UP. https://en.wikipedia.org/wiki/Two-up

It consisted of tossing a penny in the air and while it is spinning high above their heads, a punter would place a bet on it landing on the ground either heads or tails. A penny was used not only for its large size but because they knew the chances of it landing heads was exactly 50%. Since there aren't any pennies around today, (and 20c coins are just "not the same") you can make your own heads or tails predictor with the aid of electronics and learn about the laws of chance. 

## PARTS
* R5 Resii istor 10K
* R7 4K7
* R8 4K7
* R9 12OR
* 2 - 5mm Red LEDs
* 2 - diodes IN 4148
* IC2 CD 4017
* 5 - Molex pins 

This circuit is designed to have no bias, meaning it doesn't tend to favour one LED or the other. This means it can be used with confidence, which is more than could be said about the reliability of a "TWO-UP SCHOOL"...as they used trick pennies, and fluttering instead of spinning the coin! 
## MOUNTING THE PARTS
Solder the CD 4017 carefully onto the board with pin 1 passing through the correct hole. Use your fingers as a heat-sink. Follow the layout diagram to locate the positions of the 4 resistors, 2 LEDs and 2 diodes. The LEDs and diodes must be inserted around the correct way or they will not operate. Don't heat up the LEDs excessively while soldering as this will destroy their brightness. Make up 4 jumper leads from 5cm lengths of hook-up flex. Tin both ends of each lead and solder them in positions marked "J". On the jumper lead nearest the CD 4017, solder a flying Molex pi to the lead. Fit a Molex pin to the PC board in the three positions shown. Cut two short resO istor leads and insert them into the board in positions marked "W". The flying Molex pin will fit onto either of these wires to form Sw4, the clock inhibit switch. For projects 2 & 3 it is moved from wire W2 to W1 to freeze the output. For project 2 the reset jumper J4 is connected onto the Molex pin near IC2. This will allow only the first outputs to become activated.  

## HOW THE CIRCUIT WORKS
The CD 4017 is a counting IC. We are using only two of its outputs in this project. The first output is pin 3 and the second output is pin 2. It has a further 8 outputs which are not used in this project. They are by-passed by using the reset pin number 15 as follows: The third output pin 4 is connected back to the reset pin so that the IC will clock from pin 3 to pin 2 then back to pin 3 again. The input pin 14 counts the incomming pulses from the flip-flop IClaand IC1b. By rotating R2 to minimum resistance the frequency will be about 24Hz. This is the highest frequency obtainable from the flip-flop. Its range starts from one cycle per 9 seconds to 24 cycles per second. The counting IC accepts this and displays the pulses alternately at pins 3 and 2. This means each LED will flash at 12 times per second In fact it will look as if both LEDs are glowing dimly. The IC has another feature built into it at pin 13. This is called the "clock inhibit" pin. Its function is to "freeze" the output at any given instant. It comes into operation when a voltage above about 4v is applied to pin 13. To obtain positive freezing or clocking we apply either full rail voltage or zero voltage to this pin. In this project we use this "freezing" facility to give us a readout of either heads or tails. At the rate of 12 flashes per second you will be unable to deliberately stop the motion of a particular LED due to the cycling being higher than the Persistence of Vision. (Which is about 5-6Hz). Thus the freezing of either LED will be completely at random and since both LEDs are clocked on and off at an equal rate, (50% duty cycle each), there will be no bias towards either. 

 ![](https://github.com/SteveJustin1963/TE-2-46-HEADS-TAILS/blob/master/shade.png)
 ![](https://github.com/SteveJustin1963/TE-2-46-HEADS-TAILS/blob/master/larg.png)
 



  
