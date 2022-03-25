# spel-programmering-template
Mall till https://koda.nu/ js bibbliotek

Klicka på knappen fork och gör det till erat eget repo.
Ändra sedan namnet i settings till erat för- och efter namn. 

Video tutorials vi kommera att följa: https://www.youtube.com/playlist?list=PLacLTA7npkEaxlsKIL06aLqtLVKIKurRN

Notera att detta bibblioteket är grundläggande och det gör att man har mindre frihet än andra bibbliotek. 


## API

### abs(X)
Returnerar absolutbeloppet av talet X.
## arc(X, Y, RADIE, VINKEL, TJOCKLEK, FÄRG)
Ritar ett cirkelsegment på position (X, Y) med den givna radien, vinkeln, linjetjockleken och färgen.
### ceil(X)
Returnerar talet X utan några decimaler, avrundat uppåt.
### circle(X, Y, RADIE, FÄRG)
Ritar en fylld cirkel på position (X, Y) med den givna radien och färgen.
### clearScreen()
Rensar ritytan.
### distance(X1, Y1, X2, Y2)
Returnerar avståndet mellan punkterna (X1, Y1) och (X2, Y2). Kan också anropas med endast två argument om de är objekt som innehåller variablerna x och y.
### distance3D(X1, Y1, Z1, X2, Y2, Z2)
Returnerar avståndet mellan punkterna (X1, Y1, Z1) och (X2, Y2, Z2). Kan också anropas med bara två argument om de är objekt som innehåller variablerna x, y och z.
### fill(FÄRG)
Fyller ritytan med en färg.
### floor(X)
Returnerar talet X utan några decimaler, avrundat neråt.
### getPixel(X, Y)
Returnerar ett objekt som innehåller variablerna red, green och blue, som representerar färgen på den pixel som befinner sig på ### positionen (X, Y).
### hideMouse()
Döljer muspekaren.
### keyboard
Ett objekt som innehåller variabler för tangenterna på tangentbordet. Variablerna är antingen sanna eller falska beroende på om just den tangenten är nedtryckt för tillfället. De tangenter som du kan kontrollera med namn är: up, down, left, right, space, shift, alt, ctrl, enter, zero → nine, a → z. Bokstäverna stämmer bara på svenska och engelska tangentbord. Det går också att kontrollera keyboard[X], där X är koden för en viss tangent.
### line(X1, Y1, X2, Y2, TJOCKLEK, FÄRG)
Ritar ett streck från koordinaten (X1, Y1) till (X2, Y2) med den givna tjockleken och färgen.
### loopSound(LJUD, VOLYM)
Spela ett bakgrundsljud om och om igen i bakgrunden, exempelvis musik. Argumenten fungerar som i playSound som är beskrivet nedan.
### math
Ett objekt som gör det lätt att experimentera med matematik.
### mixColor(R, G, B)
Används för att blanda en egen färg. Det första argumentet anger hur mycket rött som ska blandas in, det andra anger mängden grönt och det tredje mängden blått. Varje argument ska vara mellan 0 och 255. Exempel: circle(100, 100, 50, mixColor(100, 0, 0));.
### mouse
Ett objekt som innehåller musens nuvarande position och status. Variablerna x och y ger positionen och variablerna left, right och middle ger sant eller falskt beroende på om motsvarande musknapp är nedtryckt.
### pi
En variabel som innehåller talet pi.
### picture(X, Y, BILD)
Placerar en bild på ritytan, där bildens övre vänstra hörn hamnar på position (X, Y). Argumentet BILD kan vara en webbadress eller en sökväg till en bild på datorn.
### playSound(LJUD, VOLYM)
Spela upp en ljudeffekt. Argumentet volym ska vara ett tal mellan 0 och 1; om du inte anger någon volym så blir den 1.
### pow(BAS, EXPONENT)
Returnerar ett tal som är BAS upphöjt till EXPONENT. Om man anropar funktionen med basen 2 och exponenten 3 blir resultatet: 8.
### preloadSound(LJUD)
Laddar in ett ljud i datorns minne.
### random(X)
Returnerar ett slumptal mellan 0 och X - 1.
### randomAlternative(LISTA)
Returnerar ett slumpmässigt element från en lista.
### rectangle(X, Y, BREDD, HÖJD, FÄRG)
Ritar en rektangel på koordinaten (X, Y) med den givna bredden, höjden och färgen.
### restore()
Återställer koordinatsystemet till det tillstånd som det var i vid det senaste anropet av save().
### ring(X, Y, RADIE, TJOCKLEK, FÄRG)
Ritar en ring på position (X, Y) med den givna radien, linjetjockleken och färgen.
### rotate(GRADER)
Roterar koordinatsystemet med GRADER grader.
### rotateRadians(RADIANER)
Roterar koordinatsystemet med RADIANER radianer.
### save()
Sparar koordinatsystemets nuvarande läge.
### scale(X-FAKTOR, Y-FAKTOR)
Förstorar eller förminskar hela koordinatsystemet i X- respektive Y-ledd. Om ett negativt tal anges blir koordinatsystemet spegelvänt kring den axeln.
Exempel: scale(2, 2) (allt blir dubbelt så stort)
Exempel: scale(1, -1) (allt blir upp-och-nedvänt)
### showMouse()
Gör att muspekaren blir synlig.
### sin(V) cos(V) tan(V) asin(V) acos(V) atan(V)
De vanligaste trigonometriska funktionerna sinus, cosinus, tangens samt deras inverser. Alla tar som argument en vinkel uttryckt i radianer.
### sqrt(X)
Returnerar kvadratroten av talet X.
### start()
Den första funktionen som körs.
### stopSound(LJUD)
Stoppar ett ljud om det håller på att spelas upp.
### stopUpdate()
Stoppar update()-funktionen och avslutar därmed animeringen.
### text(X, Y, STORLEK, TEXTSTRÄNG, FÄRG)
Ritar ut textsträngen TEXTSTRÄNG på koordinaten (X, Y) med den givna färgen och storleken.
### totalHeight
Den totala höjden på den tillgängliga ritytan.
### totalWidth
Den totala bredden på den tillgängliga ritytan.
### touchscreen
Ett objekt som innehåller information om användarens petskärm. Objektet innehåller variabeln currentlyTouched, som är sann eller falsk beroende på om någon petar för tillfället, samt arrayen points som innehåller de beröringspunkter som just då finns. Varje beröring har tre egenskaper, x, y och id.
### translate(X, Y)
Förflyttar koordinatsystemets origo till koordinaten (X, Y).
### triangle(X1, Y1, X2, Y2, X3, Y3, FÄRG)
Ritar en triangel som har sina hörn på koordinaterna (X1, Y1), (X2, Y2) och (X3, Y3) med den givna färgen.
turtle
Ett objekt som man kan använda för att göra så kallad turtlegrafik.
### update()
En funktion som anropas många gånger per sekund och gör det möjligt för programmeraren att skapa rörliga objekt.
### updatesPerSecond
Innehåller ett tal som anger hur många gånger per sekund som update() anropas.
