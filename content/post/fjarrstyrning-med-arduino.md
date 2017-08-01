+++
date = "2014-06-08T20:28:47Z"
draft = false
title = "FJÄRRSTYRNING MED ARDUINO"
aliases = [
    "2014/06/08/fjarrstyrning-med-arduino/"
]
+++
# FJÄRRSTYRNING MED ARDUINO
I dag köpte vi in det mesta som behövs för fjärrstyrning av trim-vingen. Vi hade en imaginär inköpslista som vi hade memorerat och gick till Kjell & Company med den. 

Med oss därifrån till en kostnad av 739 SEK ink. moms fick vi:

 - Arduino Uno
 - fjärrkontroll
 - IR-sensor
 - Arduino låda
 - Servomotor som kan dra 4,1 kg
 - USB sladd
 - 9 V Litium batteri
 - kontakt till batteriet
 - radda sockerbitar

Tidigare hade jag plöjt 10 Arduino böcker och allt som är värt att läsa på nätet i ämnet. Sen hem och börja labba.

Inkoppling och test
===================

Först gick vi till Arduino's webbsida, då det inte följer med några manualer och läste Getting started guiden. Det var till och med enklare än i guiden. I Win 7 hittades drivrutinen med en gång när jag pluggade in USB sladden mellan Uno och PC:n och installerades utan problem. Sen laddade vi in blink testet och det fungerade utan problem, rätt COM port hade ställts in automatiskt. Tidsåtgång ca 2 min.

Inkoppling av servomotorn
=========================

Vi gör allt i små steg, man vinner sällan tid på att försöka göra allt på en gång. Nu pluggade vi in servomotorn till Arduino enligt SingleServoExample. Det fungerade inte alls. Jag hade kopplat signalkabeln fel. När jag kopplade den till pinne 9 så fungerade den tillslut, servomotorns hjul roterade fram och tillbaka med 90 graders vinkel. 

Allt hade gått överraskande problemfritt och snabbt och enkelt. Total tidsåtgång med inköp, transport och tester: 1,5 h. 

Nästa steg är att koppla in IR-fjärrstyrningen och skriva ett litet program för detta, få det att fungera och och sen testa.

När det är klart så ska vi bränna ner allt till Arduinon, koppla bort USB sladden och köra på 9V litium batteriet.

Fortsättning följer...
