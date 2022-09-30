# ESERCIZIO CON LE MASCHERE VARIABILI

## Scopo e componenti utilizzate
Lo scopo dell'esercizio era collegare cinque reti fra di loro attraverso le seguenti informazioni:

le reti erano tutte di classe C, partendo dall'indirizzo 192.168.5.0;
le tre sottoreti erano formate da 28, 28, 14, 7, 2;

Per la realizzazione dell'esercizio, vengono utilizzati cinque switch (uno per rete) e cinque pc (uno per rete; numero indicativo per facilitare la realizzazioe dell'esercizio) e un router che collega gli switch tra di loro.

## Realizzazione e spiegazione
Prima di settare i pc è necessario svolgere i calcoli per capire per ogni rete indirizzo di rete, subnet mask e indirizzo di broadcast. Ecco come si procede:

- si parte dalla rete più grande;
- si calcola il numero effettivo degli host tenedo conto che deve esserci spazio indirizzo di rete e broadcast, ovvero primo e ultimo inidirizzo che non possono essere  - utilizzati (con la potenza di 2 più vicina e maggiore al valore indicato)
- trovo il numero di IP disponibili (32 - bitDellaRete, che corrisponde al valore dell'esponente nella potenza di 2)
- il primo indirizzo utile è per la rete;
- si calcola il broadcast (sommando l'ultimo valore dell'ip rete al valore di host - 1, che corrisponde al broadcast);
- si calcola la subnet mask (con il numero di IP disponibili, so che nella subnet i primi 26 valori saranno a 1 e gli altri a zero; converto e trovo la subnet);

CALCOLI.
SOTTORETE 28.
2^5 = 5 bit (32 host)
ip: 192.168.5.0 /27
rete: 192.168.5.0
broadcast: 192.168.5.31
subnet: 255.255.255.224

SOTTORETE 28.
2^5 = 5 bit (32 host)
ip: 192.168.5.0 /27
rete: 192.168.5.32
broadcast: 192.168.5.63
subnet: 255.255.255.224

SOTTORETE 14.
2^4 = 4 bit (16 host)
ip: 192.168.5.0 /28
rete: 192.168.5.64
broadcast: 192.168.5.79
subnet: 255.255.255.240

SOTTORETE 7.
2^4 = 4 bit (16 host)
ip: 192.168.5.0 /28
rete: 192.168.5.80
broadcast: 192.168.5.95
subnet: 255.255.255.240

SOTTORETE 2.
2^2 = 2 bit (4 host)
ip: 192.168.5.0 /27
rete: 192.168.5.96
broadcast: 192.168.5.99
subnet: 255.255.255.252

Svolti tutti i calcoli, posso inserire gli ip e concludere l'esercizio.
