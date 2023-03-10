# Projektseite "Schaf und Wolf"

## Konzept
Wir haben uns am Anfang überlegt, ein "Schaf und Wolf"-Brettspiel mit Greenfoot für 2-5 Spieler zu erstellen. Dabei sollte es 4 Schafe und einen Wolf geben, welcher das Ziel hat, auf die oberste Reihe schwarzer Felder zu kommen. Dabei verliert der Wolf, wenn er auf dem selben Feld wie ein Schaf ist. Die Spielfiguren können nur auf schwarzen Feldern und innerhalb des Spielfelds laufen. Wenn sie versuchen, diese zu verlassen, sterben einzelne Schafe und der Wolf verliert direkt. Die Schafe verlieren erst, wenn alle 4 tot sind oder der Wolf die oberste Reihe schwarzer Felder erreicht hat.

## Aufbau
Die Figuren stehen auf einem schwarz-weißen Brett. Es gibt einen Wolf, der von einer schwarzen Figur dargestellt wird und in der untersten schwarzen Reihe auf dem mittleren Feld beginnt. Seine Gegner sind 4 Schafe, die auf der obersten Reihe schwarzer Felder beginnen. Auf den Figuren sind die Tasten zu sehen, mit denen man sie bewegen kann. Dabei können sich Schafe nur nach unten und der Wolf nach oben und unten bewegen. Das Brett können die Figuren nicht verlassen.

## Regeln
Es gibt einige festgeschriebene Regeln.
Ziel des Wolfs ist es, die oberste Reihe schwarzer Felder zu erreichen, ohne auf dem selben Feld wie eines der Schafe zu stehen. Die einzige Ausnahme bildet die oberste Reihe schwarzer Felder. Wenn der Wolf diese betritt, gewinnt er, was am grünen Häkchen zu sehen ist.
Ziel des Teams der Schafe ist es, den Wolf zu töten. Dafür müssen sie es schaffen, dass ein Schaf auf dem selben Feld wie der Wolf steht. Wenn sie dies schaffen, gewinnen die Schafe und ein rotes Kreuz erscheint.
Für beide Teams ist es verboten, das Spielfeld zu verlassen. Wenn Schafe das versuchen, sterben sie und wenn der Wolf es versucht, verliert er direkt.
Außerdem wäre es empfehlenswert, dass der Wolf beginnt und danach Schaf und Wolf abwechselnd ziehen bis Schafe oder Wolf gewonnen haben. Wenn das grüne Häkchen erscheint, hat der Wolf gewonnen und bei dem roten Kreuz die Schafe.

## Spieloptionen
Es gibt zwei Welten, in denen man spielen kann. In der ersten Welt ist das "normale Spiel". In der zweiten Welt (SchafUndWolf2) gibt es mit dem Gnark eine weitere Spielkomponente. Dieser läuft zufällig über das Spielfeld und tötet alles, was ihm zu nahe kommt.

## Die verschiedenen Klassen/Actors erklärt

[SchafUndWolf](#1)

[SchafUndWolf2](#2)

[GameOver](#3)

[Schaf](#4)

[SchwarzStrichWin](#5)

[SchwarzerKreis](#6)

[SchwarzerKreis2](#7)

[WeißStrich](#8)

[WeißerKreis](#9)

[WeißerKreis2](#10)

[WinOver](#11)

[Wolf](#12)

[Gnark](#13)

### <a name="1"></a>SchafUndWolf
Diese Klasse ist für die Welt...
Super ist die Weltgröße, die bei 416 mal 416 liegt. 
Der Befehl Prepare legt fest, wo die verschiedenen Aktoren erschaffen werden.
Für die Schafe wird zudem die individuelle Steuerung, sowie das zugehörige Bild geladen.
![Screenshot (22)](https://user-images.githubusercontent.com/111414678/221164287-9a0e742c-46f3-454c-8eea-a69fc19b2c91.png)

![Screenshot (23)](https://user-images.githubusercontent.com/111414678/221164237-0510d77c-617e-4af6-900f-bff9a9ed9048.png)

![image](https://user-images.githubusercontent.com/111414678/221164183-ca406f2b-6411-48df-b5cb-17b05a922721.png)


### <a name="2"></a>SchafUndWolf2
Diese Klasse ist für die zweite Welt. Diese unterscheidet sich von der ersten Welt darin, dass es einen zusätzlichen Actor, den "Gnark" gibt, welcher zufällig über das Spielfeld läuft und Wolf wie auch Schafe tötet, wenn diese ihm zunahe kommen. SchafUndWolf2 ist abgeleitet von SchafUndWolf.
![image](https://user-images.githubusercontent.com/111414678/223656140-f4965825-bc02-48fd-81ed-266210b4c256.png)

### <a name="3"></a>GameOver 
Die Klasse GameOver sorgt dafür, dass bei Aktivierung ein Bild gezeigt wird, dass den Bildschirm abdeckt und ein rotes X auf schwarzem Hintergrund zeigt, das signalisiert, dass der Wolf gestorben und deshalb das Team der Schafe gewonnen hat.
![image](https://user-images.githubusercontent.com/111414678/221164569-0b41ad90-b7f8-4632-afee-d2a193a7a5f9.png)

### <a name="4"></a>Schaf 

![Screenshot (26)](https://user-images.githubusercontent.com/111414678/221164916-e1ace399-e97d-451b-bf1b-f2efed7e9108.png)


![image](https://user-images.githubusercontent.com/111414678/221164876-e38a5b9b-d5df-4c3e-98c4-6c7733c9e45e.png)

### <a name="5"></a>SchwarzStrichWin 
Dieser Actor ist einmal auf jedem schwarzen Feld auf der obersten Reihe schwarzer Felder und kann vom Wolf getötet werden, wenn dieser auf dem selben Feld. Wenn dies passiert, dann wird der "WinOver"-Actor ausgelöst und der Wolf hat gewonnen.
![image](https://user-images.githubusercontent.com/111414678/221165461-4e0cb48d-6aad-4810-a535-698005361f8e.png)

### <a name="6"></a>SchwarzerKreis 
![image](https://user-images.githubusercontent.com/111414678/221165544-3f1364eb-bfb3-4412-b6a5-cca1b20f412b.png)


### <a name="7"></a>SchwarzerKreis2 
![image](https://user-images.githubusercontent.com/111414678/221165585-9984cf5a-902a-4bfb-a623-6179260cb97c.png)


### <a name="8"></a>WeißStrich 
Der Actor WeißStrich ist einmal auf jedem weißen Feld am Rand des Spielfelds, sodass Wolf und Schafe das Spiel nicht verlassen können, da der Weißstrich-Actor beide töten, sollten diese auf dem selben Feld stehen.
![image](https://user-images.githubusercontent.com/111414678/221165623-752679c4-c8cf-40d8-b2df-bffc64adc6d6.png)

![image](https://user-images.githubusercontent.com/111414678/221165657-8eb02741-61ea-4868-8113-4b86d71a95b5.png)


### <a name="9"></a>WeißerKreis 
![image](https://user-images.githubusercontent.com/111414678/221165696-59c887ca-2349-4745-b94b-13b04427bf86.png)


### <a name="10"></a>WeißerKreis2 
![image](https://user-images.githubusercontent.com/111414678/221165756-74176a88-da6e-4523-9b15-ccb19e4b46b7.png)


### <a name="11"></a>WinOver 
Die Klasse WinOver sorgt dafür, dass bei Aktivierung ein Bild gezeigt wird, dass den Bildschirm abdeckt und ein grünes Häkchen auf schwarzem Hintergrund zeigt, das signalisiert, dass der Wolf auf die oberste Linie schwarzer Felder gekommen ist und deshalb gewonnen hat.
![image](https://user-images.githubusercontent.com/111414678/221165813-feb8c739-a295-411d-9c5b-2ceaaceac94a.png)


### <a name="12"></a>Wolf 
![image](https://user-images.githubusercontent.com/111414678/221165945-00af69eb-7916-49b0-ad6c-eb72a5ddc50d.png)
![image](https://user-images.githubusercontent.com/111414678/221165976-4c529a7e-f65f-4c9b-b4b0-711c464412fc.png)
![image](https://user-images.githubusercontent.com/111414678/221166009-7678b69e-ef02-4310-8c99-a69e3975c18d.png)

### <a name="13"></a>Gnark 
Der Gnark ist ein Actor, welcher zufällig über das Brett läuft und dabei Wolf und Schafe tötet, wenn er diesen zu nah kommt. Das sorgt dafür, dass Spieler zum Teil schneller ziehen müssen und allgemein kommt eine weitere Komponente zum Spiel dazu, welche dieses abwechslungsreicher macht.
![image](https://user-images.githubusercontent.com/111414678/223654327-623fab0e-876d-4751-8907-3ba17600e7ef.png)
![image](https://user-images.githubusercontent.com/111414678/223654387-498ed2aa-e155-4e45-8f60-08b344d8ce2e.png)
![image](https://user-images.githubusercontent.com/111414678/223658438-c4cad2b4-7720-4087-884d-41326b699b5b.png)
