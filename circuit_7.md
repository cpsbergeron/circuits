# Circuits électriques - Tutoriel 7

## @showdialog

Utilise les branchements du tutoriel précédent pour réaliser la programmation de ce tutoriel.

## @showdialog

➡️ Le circuit doit s'allumer lorsque le bouton A est pressé. 

➡️ Le circuit doit clignoter lorsque le bouton B est pressé. 

➡️ Le circuit doit s'éteindre lorsque le bouton A+B est pressé. 


## Étape 1 

Supprime les blocs ``||basic:au démarrage||`` et ``||basic:toujours||``.

## Étape 2

➡️ Le circuit doit s'allumer lorsque le bouton A est pressé. 

🚨 À l'aide de l'indice, reproduis la programmation.

🚨 Plusieurs valeurs sont incorrectes. Apporte les modifications nécessaires.

```blocks
input.onButtonPressed(Button.A, function () {
    pins.digitalWritePin(DigitalPin.P0, 0)
    pins.digitalWritePin(DigitalPin.P0, 0)
    pins.digitalWritePin(DigitalPin.P0, 0)
})
```

## Étape 3

➡️ Le circuit doit clignoter lorsque le bouton B est pressé. 

🚨 À l'aide de l'indice, reproduis la programmation.

🚨 Plusieurs valeurs sont incorrectes. Apporte les modifications nécessaires.


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

```

## Étape 4

➡️ Le circuit doit s'éteindre lorsque le bouton A+B est pressé. 

🚨 À l'aide de l'indice, reproduis la programmation.

🚨 Plusieurs valeurs sont incorrectes. Apporte les modifications nécessaires.

```blocks

input.onButtonPressed(Button.A, function () {
    pins.digitalWritePin(DigitalPin.P0, 0)
    pins.digitalWritePin(DigitalPin.P0, 0)
    pins.digitalWritePin(DigitalPin.P0, 0)
})

```

## @showdialog 

Félicitations! Tu as terminé de programmer un circuit électrique avec plusieurs lumières LED.

Essaie de brancher l'ensemble des composantes du circuit sans indice.

Pour tester le circuit électrique, télécharge la programmation dans le micro:bit.


