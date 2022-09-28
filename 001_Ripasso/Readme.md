# ESERCIZIO DI RIPASSO IN CISCO PACKET TRACER

## Scopo e componenti utilizzate
Lo scopo dell'esercizio era quello di creare due reti e farle comunicare attraverso l'utilizzo di un router.
Le due reti sono entrambe composte da due pc e uno switch per ogni rete.
Oltre ai componenti sopraelencati, viene collegato un router tra i due switch per metterli in comunicazione.

## Realizzazione e spiegazione
Le reti vengono settate con i classici indirizzi iPv4 di inidirizzi 192.168.0.x e 192.168.1.x.
Per far comunicare le reti, abbiamo inizialmente settato tutti gli indirizzi iPv4 al singolo PC, lasciando la subnet mask suggerita dal programma.
Successivamente, sempre er ogni computer presente, abbiamo inizializzato il default gateway, ovvero l'indirizzo a cui mandare i messaggi nel caso in cui il destinatario non sia nella stessa rete del mittente: per la prima rete, abbiamo utilizzato il 192.168.0.254, per la seconda invece 192.168.1.254.

Nel router sono stati aggiunti come indirizzi iPv4 dei cavi che collegano le reti gli stessi indirizzi default gateway delle reti stesse, in modo che se un mittente non trova il proprio destinatario spedisce al router il messaggio, il quale si occupa di smistarlo nella rete corretta.
