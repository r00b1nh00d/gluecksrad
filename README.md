# Glücksrad
## ~avatar avatar @unplugged
Wer ist dran mit auspacken? <br>
![Gluecksrad](https://github.com/r00b1nh00d/gluecksrad/blob/master/Gluecksrad.gif?raw=true)
## ~ @unplugged 
Lass den Calliope per Zufall entscheiden in welcher Reihenfolge ihr eure Weihnachtsgeschenke auspackt.


## Schritt 1
Erstelle  ``||basic:beim Start||`` eine ``||arrays:Liste||``. Auf dieser Liste kannst du Pfeile in Bilderform speichern, dazu gibt es bis beim Calliope bis zu acht.
```blocks
let Glücksrad: Image[] = []
Glücksrad = [images.iconImage(IconNames.ArrowNorth), images.iconImage(IconNames.ArrowNorthEast), images.iconImage(IconNames.ArrowEast), images.iconImage(IconNames.ArrowSouthEast), images.iconImage(IconNames.ArrowSouth), images.iconImage(IconNames.ArrowSouthWest), images.iconImage(IconNames.ArrowWest), images.iconImage(IconNames.ArrowNorthWest)]

```

## Schritt 2
Wenn du jetzt den ``||inputs: Knopf A||`` drückst soll es wie bei einem Glücksrad aussehen, als ob sich der Pfeil auf dem Bildschirm dreht.<br>
Dazu sollen die Bilder aus der Liste nach und nach angezeigt werden. Mit einer ``||loops:index Schleife||`` und dem Block ``||images:zeige Bild||`` kannst du dir, die in der Liste gespeicherten Bilder nach und nach anzeigen lassen. <br>
Mit einer ausgeklügelten  Programmierung des ``||math:Zufalls||`` bleibt der Pfeil immer bei einer anderen Position stehen. 

```blocks
input.onButtonPressed(Button.A, function () {
    for (let Index = 0; Index <= randint(32, 40); Index++) {
        Glücksrad[Index % 8].showImage(0)
    }
})
let Glücksrad: Image[] = []
Glücksrad = [images.iconImage(IconNames.ArrowNorth), images.iconImage(IconNames.ArrowNorthEast), images.iconImage(IconNames.ArrowEast), images.iconImage(IconNames.ArrowSouthEast), images.iconImage(IconNames.ArrowSouth), images.iconImage(IconNames.ArrowSouthWest), images.iconImage(IconNames.ArrowWest), images.iconImage(IconNames.ArrowNorthWest)]
```

