# Glücksrad
## ~avatar avatar @unplugged
Wer ist dran mit auspacken?
gedulde dich noch ein wenig bis es soweit ist :-)

nput.onButtonPressed(Button.A, function () {
    for (let Index = 0; Index <= randint(32, 40); Index++) {
        Glücksrad[Index % 8].showImage(0)
    }
})
let Glücksrad: Image[] = []
Glücksrad = [images.iconImage(IconNames.ArrowNorth), images.iconImage(IconNames.ArrowNorthEast), images.iconImage(IconNames.ArrowEast), images.iconImage(IconNames.ArrowSouthEast), images.iconImage(IconNames.ArrowSouth), images.iconImage(IconNames.ArrowSouthWest), images.iconImage(IconNames.ArrowWest), images.iconImage(IconNames.ArrowNorthWest)]
