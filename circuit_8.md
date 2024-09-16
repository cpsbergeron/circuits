# Circuits électriques - Tutoriel 8

## @showdialog

🌈🌈🌈 Utilise la LED arc-en-ciel pour réaliser ce tutoriel. 🌈🌈🌈

## Étape 1
 
Crée une ``|| variables: variable  ||`` et donne lui le nom ``|| variables: circuit  ||``. 

Ajoute le bloc ``|| variables: définir circuit ||`` dans le bloc ``|| basic: toujours  ||``.

```blocks

let circuit = 0
	
})

```

## Étape 2
 
Glisse le bloc ``|| input: lorsque le bouton A est pressé ||`` dans la zone de programmation.

Ajoute le bloc ``|| variables: modifier circuit ||`` dans le bloc ``|| input: lorsque le bouton A est pressé   ||``.

Remplace la valeur ``|| variables: 0 ||`` du bloc ``|| variables: modifier circuit ||`` par ``|| variables: 1 ||``.

```blocks

let circuit = 0
input.onButtonPressed(Button.A, function () {
    circuit += 1
})

```

## Étape 3
 
Ajoute le bloc ``|| basic: montrer nombre ||`` sous le bloc ``|| variables: modifier circuit ||``.

Remplace la valeur ``|| basic: 0 ||`` du bloc ``|| basic: montrer nombre ||`` par le bloc ``|| variables: circuit   ||``.

```blocks

let circuit = 0
input.onButtonPressed(Button.A, function () {
    circuit += 1
    basic.showNumber(circuit)

})

```

## Étape 4
 
Glisse le bloc ``|| input: lorsque le bouton B est pressé ||`` dans la zone de programmation.

Ajoute le bloc ``|| variables: modifier circuit ||`` dans le bloc ``|| input: lorsque le bouton B est pressé   ||``.

Remplace la valeur ``|| variables: 0 ||`` du bloc ``|| variables: modifier circuit ||`` par ``|| variables: -1 ||``.

```blocks

let circuit = 0
input.onButtonPressed(Button.B, function () {
    circuit += -1
})

```

## Étape 5
 
Ajoute le bloc ``|| basic: montrer nombre ||`` sous le bloc ``|| variables: modifier circuit ||``.

Remplace la valeur ``|| basic: 0 ||`` du bloc ``|| basic: montrer nombre ||`` par le bloc ``|| variables: circuit   ||``.

```blocks

let circuit = 0
input.onButtonPressed(Button.B, function () {
    circuit += -1
    basic.showNumber(circuit)
})

```

## Étape 6
 
Ajoute le bloc ``|| logic: si alors sinon ||`` dans le bloc ``|| basic: toujours ||``.

```blocks

basic.forever(function () {
    if (true) {
    	
    } else {
    	
    }
})

```

## Étape 6
 
Modifie le bloc ``|| logic: si alors sinon ||``.

Remplace la valeur ``|| logic: vrai ||`` par le bloc ``|| logic: 0 = 0 ||``.


```blocks

basic.forever(function () {
    if (0 == 0) {
    	
    } else {
    	
    }
})

```

## Étape 7

Remplace la valeur ``|| logic: 0 ||`` de gauche par le bloc ``|| variables: circuit ||``.

Remplace la valeur ``|| logic: 0 ||`` de droite par la valeur ``|| logic: 1 ||``.

```blocks

let circuit = 0
basic.forever(function () {
    if (circuit == 1) {
    	
    } else {
    	
    }
})

```

## Étape 7

Ajoute le bloc ``|| loops: répéter ||`` dans le bloc ``|| logic: si ||``

```blocks

let circuit = 0
basic.forever(function () {
    if (circuit == 1) {
        for (let index = 0; index < 4; index++) {
        	
        }
    } else {
    	
    }
})

```

## Étape 8

Ajoute trois blocs ``|| pins: écrire sur la broche ||`` dans le bloc ``|| loops: répéter ||``

```blocks

let circuit = 0
basic.forever(function () {
    if (circuit == 1) {
        for (let index = 0; index < 4; index++) {
            pins.digitalWritePin(DigitalPin.P0, 0)
            pins.digitalWritePin(DigitalPin.P0, 0)
            pins.digitalWritePin(DigitalPin.P0, 0)
        }
    } else {
    	
    }
})

```

## @showdialog

🚨 Plusieurs valeurs sont incorrectes. Apporte les modifications nécessaires.

Une seule LED doit clignoter. (P0)

## Étape 9

Ajoute le bloc ``|| basic: pause ||`` sous les les blocs ``|| pins: écrire sur la broche ||``.

```blocks

let circuit = 0
basic.forever(function () {
    if (circuit == 1) {
        for (let index = 0; index < 4; index++) {
            pins.digitalWritePin(DigitalPin.P0, 0)
            pins.digitalWritePin(DigitalPin.P0, 0)
            pins.digitalWritePin(DigitalPin.P0, 0)
            basic.pause(100)
        }
    } else {
    	
    }
})

```
## @showdialog

🚨 Plusieurs valeurs sont incorrectes ou manquantes. Apporte les modifications nécessaires.

Reproduis la programmation pour qu'une deuxième LED clignote (P1).

## @showdialog

🚨 Plusieurs valeurs sont incorrectes ou manquantes. Apporte les modifications nécessaires.

Reproduis la programmation pour qu'une troisième LED clignote (P2)

## Étape 10

Ajoute trois blocs ``|| pins: écrire sur la broche ||`` dans le bloc ``|| logic: sinon ||``

```blocks

let circuit = 0
basic.forever(function () {
    if (circuit == 1) {
        for (let index = 0; index < 4; index++) {
            pins.digitalWritePin(DigitalPin.P0, 0)
            pins.digitalWritePin(DigitalPin.P0, 0)
            pins.digitalWritePin(DigitalPin.P0, 0)
            basic.pause(100)
        }
    } else {
        pins.digitalWritePin(DigitalPin.P0, 0)
        pins.digitalWritePin(DigitalPin.P0, 0)
        pins.digitalWritePin(DigitalPin.P0, 0)
    }
})

```
## @showdialog

🚨 Plusieurs valeurs sont incorrectes. Apporte les modifications nécessaires.

Les trois LEDs doivent être éteintes si ``|| logic: la condition ||`` n'est pas respectée.