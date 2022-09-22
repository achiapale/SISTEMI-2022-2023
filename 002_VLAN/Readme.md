# ESERCIZIO CON LE VLAN E IL COLLEGAMENTO ACCESS

## Scopo e componenti uilizzate
Lo scopo dell'esercizio era creare due VLAN utilizzando due switch attraverso il metodo di collegamento access.
Il primo switch viene collegato a quattro pc.
Il secondo switch, oltre ad essere collegato all'altro switch, viene colegato ad altri due pc.

## Realizzazione e spiegazione
I computer vengono settati con il classici iPv4 (192.168.1.x).
Due computer dello switch 1 vengono collegati alla VLAN 10 (robotici), gli altri due alla VLAN 20 (informatici).
I pc del secondo switch vengono collegati uno alla VLAN 10 e uno alla VLAN 20.
Per creare le VLAN, è stato necessario creare nello switch nella sezione VLAN database le due nuove VLAN: 10 robotica, 20 informatica.
Successivamente sono state impostate la VLAN dalle fast ethernet che collegano i pc agli switch.

Per collegare i due switch abbiamo tirato due cavi di collegamento, uno per ogni VLAN, e successivamente le abbiamo settate assegnando il valore di ogni VLAN al singolo cavo.

L'esercizio è funzionante, ma il problema si può porre nel momento in cui ho un numero elevato di VLAN, quindi quando devo collegare tra i due switch switch molti cavi.
