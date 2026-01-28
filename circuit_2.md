# Circuits électriques - Tutoriel 2

## @showdialog

Dans ce tutoriel, tu vas programmer ton micro:bit 💻 et créer un circuit électrique 🔌 où les boutons 🅰️ et 🅱️ serviront à allumer et à éteindre une DEL (LED) 💡.

## Étape 1 

Supprime les blocs ``||basic:au démarrage||`` et ``||basic:toujours||``.

🗑️ Tu n'en auras pas besoin pour ce programme.

## Étape 2

 Glisse le bloc ``|| input: lorsque le bouton A est pressé ||`` dans la zone de programmation.

Ajoute le bloc ``|| pins: écrire sur la broche ||`` dans le bloc ``|| input: lorsque le bouton A est pressé ||``.

```blocks

input.onButtonPressed(Button.A, function () {
    pins.digitalWritePin(DigitalPin.P0, 0)
})

```

## Étape 3

Modifie les valeurs du bloc ``|| pins: écrire sur la broche ||``.

Remplace la broche ``|| pins: P0 ||`` par ``|| pins: P1 ||``.

Remplace la valeur ``|| pins: 0 ||`` par ``|| pins: 1 ||``.

La valeur 1 envoie un signal 🔆 allumé à la broche P1.

```blocks

input.onButtonPressed(Button.A, function () {
    pins.digitalWritePin(DigitalPin.P1, 1)
})

```

## Étape 4

 Glisse le bloc ``|| input: lorsque le bouton B est pressé ||`` dans la zone de programmation.

Ajoute un nouveau bloc ``|| pins: écrire sur la broche ||`` dans le bloc ``|| input: lorsque le bouton B est pressé ||``.


```blocks

input.onButtonPressed(Button.B, function () {
    pins.digitalWritePin(DigitalPin.P0, 0)
})

```

## Étape 5

Modifie les valeurs du bloc ``|| pins: écrire sur la broche ||``.

Remplace la broche ``|| pins: P0 ||`` par ``|| pins: P1 ||``.

La valeur ``|| pins: 0 ||`` demeure la même.

Ce bloc envoie un signal 0 (💤 éteint) sur la broche P1.

```blocks

input.onButtonPressed(Button.B, function () {
    pins.digitalWritePin(DigitalPin.P1, 0)
})

```

## @showdialog 

🔌 Reproduis le branchement ci‑dessous.
🎨 La couleur des fils n'a pas d'importance!

![MicroSeb](https://github.com/sbergeroncp/micro-seb/blob/master/2.png?raw=true)

## @showdialog 

🎉🎉🎉
➡️ Bravo! Tu viens de programmer un circuit électrique contrôlé par les boutons 🅰️ et 🅱️.

Pour tester  :

📥 Télécharge ton programme dans le micro:bit.
👆 Appuie sur A pour allumer la LED.
👆 Appuie sur B pour l'éteindre.
✨ Observe ton circuit en action!