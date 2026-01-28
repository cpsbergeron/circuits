# Circuits électriques

# Tutoriel 1

## @showdialog

Dans ce tutoriel, tu vas programmer un micro:bit et réaliser un petit circuit électrique pour allumer une lumière DEL (LED).

🚨 Lis bien chaque étape avant de continuer! 🚨

## Étape 1

Supprime le bloc ``||basic:au démarrage||``.
Tu n'en auras pas besoin.

## Étape 2

Ajoute le bloc ``|| pins: écrire sur la broche ||`` dans le bloc ``||basic: toujours||``.

Ce bloc envoie un signal de valeur 0 (donc éteint) sur la broche P0.

```blocks

basic.forever(function () {
    pins.digitalWritePin(DigitalPin.P0, 0)
})

```

## Étape 3

Modifie les valeurs du bloc ``|| pins: écrire sur la broche ||``.

Remplace la valeur ``|| pins: 0 ||`` par ``|| pins: 1 ||``.

La valeur 1 envoie un signal allumé à la broche P0.

```blocks

basic.forever(function () {
    pins.digitalWritePin(DigitalPin.P0, 1)
})

```

## @showdialog 

Reproduis le branchement illustré ci-dessous.

➡️ La couleur des fils n'a aucune importance!

![MicroSeb](https://github.com/sbergeroncp/micro-seb/blob/master/1.png?raw=true)

## @showdialog 

🎉🎉🎉

✅ Tu viens de programmer ton premier circuit électrique avec une LED!

Pour tester ta séqeunce de programmation et tes branchements :
➡️Télécharge ton programme dans le micro:bit.
➡️ Observe la LED s'allumer grâce à ta programmation!