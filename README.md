# Stap 1 - Begin

Zorg er allereerst voor dat je de Arduino IDE hebt geïntstalleerd. De versie die ik gebruik is **v2.0.0**.
Ik maak gebruik van de NodeMCU 1.0 ESP-12E Module. 

Zorg er ook voor dat je de juiste poort selecteert, anders kun je geen bestanden uploaden naar je board. 

# Stap 2 - Library installeren

Open de Library Manager van Arduino IDE.  
<img src="images\libmanager.png" width="200px" alt="de library manager van Arduino IDE">

Zoek in de zoekbalk naar "Adafruit IO Arduino" en installeer "Adafruit AW9523".  
<img src="images\libmanager2.png" width="200px" alt="de library manager van Arduino IDE met zoekbalk">

Klik daarna op 'install all'.  
<img src="images\install_all.png" width="375px" alt="install all">

De installatie is gelukt als je deze melding te zien krijgt.  
<img src="images\install_succes.png" width="200px" alt="install success">

# Stap 3 - Adafruit IO
Maak op https://io.adafruit.com/ een **gratis** account aan. 

Kopieer vanuit je account je username en je key.  

**LET OP!** 
Je vind je username en key **NIET** op de pagina waar je na het maken van je account op beland, maar ga terug naar io.adafruit.com en klik op de gele sleuter rechtsbovenin je scherm. 

# Stap 4 - Color Picker maken
Maak op https://io.adafruit.com/ een nieuw dashboard aan en ga vervolgens naar dit dashboard. 

In het dropdown-menu met het tandwiel druk je op "New Block" en kies de Color Picker.  
Tijdens het proces moet je een nieuwe feed aanmaken. Noem deze Color.

anthonie_meijers
aio_lpnk317H10vV84ZWvOJk2j1Z19t0

# Stap 5 - Code
Volg de onderstaande stappen:
1. In Arduino: File > Examples > Adafruit IO Arduino > Adafruitio_14_neopixel
2. In tab ‘config.h’: plak je Adafruit IO username en Key in
3. In tab ‘config.h’: voer het wifi netwerk en wachtwoord in 
    1. (De NodeMCU werkt niet op 5Ghz WiFi)
    2. Gebruik liefst de hotspot van je telefoon, dit gebruikt < 0.1 Mb data per uur, dus niet bang zijn
4. in de Tab adafruit_14_Neopixel.ino
    1. Pas: #define PIXEL_PIN 5 aan naar #define PIXEL_PIN D5
