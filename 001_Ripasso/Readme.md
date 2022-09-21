# ESERCIZIO DI RIPASSO IN CISCO PACKET TRACER

## Impostazione dell'esercizio
Lo scopo dell'esercizio era quello di creare due reti e farle comunicare attraverso l'utilizzo di un router.
La prima rete è composta da due pc, con indirizzi 192.168.0.10 e 192.168.0.20;
la seconda rete, con lo stesso numero di device, è invece costituita dagli indirizzi 192.168.1.10 e 192.168.1.20.
Per la comunicazione delle due reti, oltre all'utilizzo del router, vengono anche utilizzati due switch, i quali uniscono i due componenti della rete al router centrale.

## Realizzazione e spiegazione
Per far comunicare le reti, abbiamo inizialmente settato tutti gli indirizzi iPv4 al singolo PC, lasciando la subnet mask suggerita dal programma.
Successivamente, sempre er ogni computer presente, abbiamo inizializzato il default gateway, ovvero l'indirizzo a cui mandare i messaggi nel caso in cui il destinatario non sia nella stessa rete del mittente: per la prima rete, abbiamo utilizzato il 192.168.0.254, per la seconda invece 192.168.1.254.

Nel router sono stati aggiunti come indirizzi iPv4 dei cavi che collegano le reti gli stessi indirizzi default gateway delle reti stesse, in modo che se un mittente non trova il proprio destinatario spedisce al router il messaggio, il quale si occupa di smistarlo nella rete corretta.
