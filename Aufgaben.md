# Bit
## 1. Umrechnung 11111111B in Dezimal
255
## 2. Umrechnung 01001101B in Dezimal
77
## 3. Wieviele Bit werden benötigt, um 16 Bitkombinationen zu erstellen?
4 Bit = 16 Kombinationen
## 4. Umrechnung 11111111B in Hexadezimal
FF^H
## 5. Umrechnung 10110101B in Hexadezimal
B5
## 6. Umrechnung FF^H in Binär 
11111111
## 7. Umrechnung E7H in Binär 
1110'0111
## 8. Umrechnung 37D in Binär 
Mit Division: 0010'0101
## 9. Wieviele Bit werden mindestens benötigt, um 1000 Bitkombinationen darzustellen?
10 Bit = 1024

# Aufgaben Negieren

## 1. Addiere die beiden 4Bit Integer 0101B + 0011B

0101B
0011B
-----
1000B
## 2. Addiere die beiden 4Bit Integer 1101B + 0110B
1101B
0110B
-----
0011B (Dataoverflow!)
## 3. Umrechnung -4D in Unsigned Integer mit Bitbreite 4
1100B
## 4. Umrechnung -18D in Unsigned Integer mit Bitbreite 8
1110'1110B

## 1. Welche Speicherkapazität in kiB (Hinweis: 1kiB=1024B) besitzt ein Arbeitsspeicher mit 12-Bit-Adressbus und 16-Bit-Datenbus?
12Bit Adresse ergibt 212 oder 4096 Speicherplätze. Pro Speicherplatz 2B ergibt 8192Byte. In KiBi ausgedrückt: 8192/1024= 8kiBi
## 2. Zwei Geräte sind mit einer seriellen Leitung und einer Leitung für das Taktsignal von 1MHz verbunden.
 ### a. Wie viele Bytes können pro Sekunde übertragen werden?
 1MHz = 1'000'000 Hz. Somit 1'000’000Bit pro Sekunde oder 125kB/s
 ### b. Wie viele Bytes pro Sekunde können übertragen werden, wenn die Verbindung der beiden Geräte nicht seriell, sondern 8 Bit-parallel wäre?
  8x mehr. Somit 1MB/s




## Wo wird UTF8 eingesetzt, wo UTF-16?
UTF8: Internetprotokolle, UTF16:  .Net-Framework, Java, Tcl
## Was bedeutet die Byteorder bei UTF-16?
 Big Endian (UTF-16BE), Little Endian (UTF-16LE)
 UTF16-BE-BOM: FE FF… UTF16-LE-BOM: FF FE…  
## Was bedeutet «abwärtskompatibel» im Zusammenhang mit UTF-8? Existiert diese «Abwärtskompatibilität» auch bei UTF-16?
 Die ersten 128 Unicodezeichen (U+0000 bis U+007F entsprechen den Positionen 0–127 in allen
 ISO-8859-Varianten (7-Bit-ASCII). In UTF-8 deckungsgleich als ein Byte dargestellt.
 Bei UTF16 existiert dies nicht.
## Wie beurteilen sie den Speicherbedarf von deutsch- oder englischsprachigem Text bei ISO-8859-Codierung, UTF-8-Codierung und UTF-16-Codierung?
ISO-8859-Codierung und UTF-8-Codierung ist effizienter, weil UTF16 immer 2Byte belegt.
## Wann wird ein UTF-16-Code vier Byte lang?
 Unicode-Zeichen außerhalb der BMP (U+10000 bis U+10FFFF).  BMP=Basic Multilingual Plane
## Wie müssen sie vorgehen, wenn sie z.B. in Word ein Zeichen eingeben wollen, das sie auf der Tastatur zwar nicht finden, dessen Unicode sie aber kennen? (z.B. das Eurozeichen)
 U+20AC eingeben, danach ALT-C drücken.
## Was wird das Problem sein, wenn sie auf dieselbe Weise wie in der vorangegangenen Aufgabe das Unicode-Zeichen des Violinschlüssels (U+1D11E) in eine Wordtext einfügen wollen?
 Gewählter Font-Satz wie z.B. Arial enthält Violinzeichen nicht.


## 1.Wie lautet der ANSI-ASCII-Code für das Eurozeichen €? 
0x80 oder 1000’0000
## 2.Wie lautet der Unicode für das Eurozeichen €? 
U+20AC oder 0010’0000 1010’1100

## 3.Schreiben sie den ANSI-ASCII Text €URO in HEX und in Binär.
HEX: 80 55 52 4F
Binär: 10000000 01010101 01010010 01001111

## 4. Schreiben sie den UTF-8 Text €URO in HEX und in Binär.
HEX: E2 82 AC 55 52 4F
Binär: 11100010 10000010 10101100 01010101 01010010 01001111
## 5. Schreiben sie den UTF-16-BE Text €URO in HEX und in Binär.
HEX: 20 AC 00 55 00 52 00 4F

## 6. Schreiben sie den UTF-16-LE Text €URO in HEX und in Binär.
HEX: AC 20 55 00 52 00 4F 00

## 7. Vergleichen sie die Resultate.
ANSI-ASCII und UTF-8 sind sehr ähnlich, aussert beim Eurozeichen.
Bei BE-16 und LE-16 unterscheiden sich bei FE-FF und pro 16-Bit-Charakter die 
Byte-Order.
