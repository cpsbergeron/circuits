# Circuits électriques - Tutoriel 7

## @showdialog

Utilise la LED arc-en-ciel pour réaliser le défi et 6 pinces crocodiles.

## @showdialog

Plusieurs valeurs sont incorrectes. Apporte les modifications nécessaires.

## Étape 1

Utilise l'indice pour reproduire la programmation.

```blocks

input.onButtonPressed(Button.A, function () {
    for (let index = 0; index < 4; index++) {
        pins.digitalWritePin(DigitalPin.P0, 0)
        pins.digitalWritePin(DigitalPin.P0, 0)
        pins.digitalWritePin(DigitalPin.P0, 0)
        basic.pause(200)
        pins.digitalWritePin(DigitalPin.P0, 0)
        pins.digitalWritePin(DigitalPin.P0, 0)
        pins.digitalWritePin(DigitalPin.P0, 0)
        basic.pause(200)
    }
})
input.onButtonPressed(Button.AB, function () {
    pins.digitalWritePin(DigitalPin.P0, 0)
    pins.digitalWritePin(DigitalPin.P0, 0)
    pins.digitalWritePin(DigitalPin.P0, 0)
})
input.onButtonPressed(Button.B, function () {
    pins.digitalWritePin(DigitalPin.P0, 0)
    pins.digitalWritePin(DigitalPin.P0, 0)
    pins.digitalWritePin(DigitalPin.P0, 0)
})

```

## Étape 2

Apporte les modifications nécessaires.

Le circuit doit s'allumer lorsque le bouton A est pressé.
Le circuit doit clignoter lorsque le bouton B est pressé.
Le circuit doit s'éteindre lorsque le bouton A+B est pressé.

```blocks

input.onButtonPressed(Button.A, function () {
    for (let index = 0; index < 4; index++) {
        pins.digitalWritePin(DigitalPin.P0, 0)
        pins.digitalWritePin(DigitalPin.P0, 0)
        pins.digitalWritePin(DigitalPin.P0, 0)
        basic.pause(200)
        pins.digitalWritePin(DigitalPin.P0, 0)
        pins.digitalWritePin(DigitalPin.P0, 0)
        pins.digitalWritePin(DigitalPin.P0, 0)
        basic.pause(200)
    }
})
input.onButtonPressed(Button.AB, function () {
    pins.digitalWritePin(DigitalPin.P0, 0)
    pins.digitalWritePin(DigitalPin.P0, 0)
    pins.digitalWritePin(DigitalPin.P0, 0)
})
input.onButtonPressed(Button.B, function () {
    pins.digitalWritePin(DigitalPin.P0, 0)
    pins.digitalWritePin(DigitalPin.P0, 0)
    pins.digitalWritePin(DigitalPin.P0, 0)
})

```

## @showdialog 

Félicitations! Tu as terminé de programmer un circuit électrique avec plusieurs lumières LED.

Essaie de brancher l'ensemble des composantes du circuit sans indice.

Pour tester le circuit électrique, télécharge la programmation dans le micro:bit.