# ESERCIZIO CON LE MASCHERE VARIABILI

## Scopo e componenti utilizzate
Loscopo dell'esercizio era collegare tre reti fra di loro attraverso le seguenti informazioni:
- le reti erano tutte di classe C, partendo dall'indirizzo 192.168.0.0;
- le tre sottoreti erano formate da 10, 30 e 50 host;

Per la realizzazione dell'esercizio, vengono utilizzati tre switch (uno per rete) e tre pc (uno per rete; numero indicativo per facilitare la realizzazioe dell'esercizio) e un router che collega i tre switch tra di loro.

## Realizzazione e spiegazione
Prima di settare i pc è necessario svolgere i calcoli per capire per ogni rete indirizzo di rete, subnet mask e indirizzo di broadcast.
Ecco come si procede:
- si parte dalla rete più grande (in questo caso quella da 50);
- si calcola il numero effettivo degli host tenedo conto che deve esserci spazio indirizzo di rete e broadcast, ovvero primo e ultimo inidirizzo che non possono essere utilizzati (con la potenza di 2 più vicina e maggiore al valore indicato)
- trovo il numero di IP disponibili (32 - bitDellaRete, che corrisponde al valore dell'esponente nella potenza di 2)
- il primo indirizzo utile è per la rete;
- - si calcola il broadcast (sommando l'ultimo valore dell'ip rete al valore di host - 1, che corrisponde al broadcast);
- si calcola la subnet mask (con il numero di IP disponibili, so che nella subnet i primi 26 valori saranno a 1 e gli altri a zero; converto e trovo la subnet);

CALCOLI.

- SOTTORETE 50.
64 host -> 2^6 (6 bit)
ip: 192.168.0.0 /26 (32 - 6 = 26)
rete: 192.168.0.0
broadcast: 192.168.0.63 (0 + (64 - 1))
subnet: 11111111.11111111.11111111.11000000
subnet convertita: 255.255.255.192

- SOTTORETE 30.
32 host -> 2^5 (5 bit)
ip: 192.168.0.0/27
rete: 192.168.0.64
broadcast: 192.168.0.95
subnet: 255.255.255.240

- SOTTORETE 10.
16 host -> 2^4 (4 bit)
ip: 192.168.0.0 /28
rete: 192.168.0.96
broadcast: 192.168.0.111
subnet: 255.255.255.224

Svolti tutti i calcoli, posso inserire gli ip e concludere l'esercizio.
