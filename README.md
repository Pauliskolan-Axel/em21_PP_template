Här är en lista på de “Issues” du ska skapa i ditt repo på Github. Hovra över raden, och klicka på cirkeln med pricken i till höger för att omvandla till ett nytt Issue.  ladda om sidan om du inte ser cirkeln.

Varje Issue får ett nummer som du kan använda i VS code när du commit:ar. 
[https://code.visualstudio.com/blogs/2020/05/06/github-issues-integration](url)

E:
- [ ] [Feature] Send fuel gauge data to AIO.
- [ ] [Feature] Deep sleep fixed time 10 minutes.
- [ ] Blinka LED på olika sätt vid a) försöker koppla upp sig b) uppkopplad. Gör en egen funktion blinkLED(times, speed).
- [ ] Löda laddare
- [ ] Versionskontroll via Github. Jag fixar ett repo när  du har ett github-konto.

D:
- [ ] Löda OLED
- [ ] [Feature] OLED med auto-off. Visa datan i textsize 2 på två "frames" i 1,5 sekunder vid Reset-tryck.
- [ ] Ta  hänsyn till om fuelgauge.begin() inte funkar, försök några gånger. Meddela på OLED om det inte lyckas.
- [ ] [Feature] Variabel sleep time m.a.p. batteriprocent. 
> - Under 3%: 20 minuter. 
> - 3-6 %: 15 minuter. 
>  - Annars 10 minuter.

C:
- [ ] Löda INA219
- [ ] [Feature] INA219 laddningsmätare, medelvärde på 1000 samples, skicka upp till AIO.
- [ ] [Feature] Avbryt om du inte får WiFi-kontakt, skicka upp antal gånger det hänt. RTC memory. Sleep 30 sekunder. När du väl får kontakt, blinka LED:en på något unikt sätt. 
- [ ] [Feature] OLED med typsnitt.
- [ ] Dela dina feeds på AIO med mig. AIO användarnamn: **axelmagnus**

B:
- [ ] Om  spänningen är väldigt låg, (<3.4 V), ska den inte försöka sätta i gång WiFi, utan gå tillbaka i sleep och bara ladda batterier.
- [ ] Ta hänsyn till att om någon av dina I2C komponenter inte lyckas starta (.begin() ), försök några gånger med kort sleep, och sedan skicka RTC-lagrade värden i stället.
- [ ] [Feature] EXT wakeup: använd en knapp för att vakna och visa all data på OLED (men koppla upp WiFi). Konstant uppdateringstid till AIO, trots knapptryck .


A:
- [ ] [Feature] Skicka meddelande om batteriet understiger viss nivå. Se [IFTTT](https://learn.adafruit.com/using-ifttt-with-adafruit-io/ifttt-to-adafruit-io-setup).
- [ ] Längre sleep time mellan 18-06, hämta tid från AIO.
