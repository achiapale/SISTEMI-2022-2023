# ESERCIZIO CON LE VLAN E IL COLLEGAMENTO TRUNK

## Scopo e componenti utilizzate
Lo scopo era far comunicare due VLAN attraverso un collegamento di tipo trunk.
Per farlo, abbiamo utilizzato nella prima rete 4 pc con uno switch; nella seconda, invece, abbiamo uno switch e due pc.
Gli switch delle due VLAN sono stati collegati tra di loro.

## Realizzazione e spiegazione
I device sono setttati con i classici indirizzi iPv4 (192.168.1.x).
Due computer dello switch 1 vengono collegati alla VLAN 10 (robotici), gli altri due alla VLAN 20 (informatici). i pc del secondo switch vengono collegati uno alla VLAN 10 e uno alla VLAN 20.
Per creare la VLAN, è stato necessario creare negli switch (nella sezione VLAN database) due nuove VLAN: 10 robotica, 20 informatica. Successivamente sono state impostate le VLAN delle fast ethernet che collegano i pc agli switch.

Per collegare le VLAN attraverso il metodo trunk, è necessario entrare in ognuno dei due switch e dentro alle impostazioni della fast ethernet opportuna selezionare la modalità "trunk" (il collegamento effettivo verrà fatto direttamente dall'applicazione).
