# Obligatorisk oppgave 3 i Algoritmer og Datastrukturer

Denne oppgaven er en innlevering i Algoritmer og Datastrukturer. 
Oppgaven er levert av følgende student:
*  Mohanad Al-Falah, S362092, s362092@oslomet.no

Jeg har samarbeidet litt med andre for noen oppgaver.

# Oppgavebeskrivelse

I oppgave 1 Jeg har kopierete koden 5.2.3a fra kompediet, men jeg fikk feil når jeg testet koden på p = new Node <>(verdi), på konstruktøren til Node<T> på kildekode er det to parametre (verdi og forealderen). På koden er q foralder, så testet jeg oppgaven og fikk riktig svar. På koden brukes to nodereferanse p,q. Referansen P starter i rotnode, den flyttes på nedover i treet venstre om verdi er mindre, og høyre om verdi er større, så brukte jeg Compare-metoden for å sammenligne. q skal passere p og blir siste noden, da skal den nye verdi legges og sammenlignes med q og setter som barn, enten til høyre eller til venstre.

I oppgave 2 Jeg har laget kode for metoden public int antall(T verdi), denne metoden skal returnere antall forekomster av verdi i treet. Det er tillatt med duplikater og det betyr at en verdi kan forekomme flere ganger. Hvis verdi ikke er i treet (null er ikke i treet), skal metoden returnere 0.

I oppgave 3 jeg har kopierte koden 5.7.1 fra kompediet, og har byttet if (tom()) throw new NoSuchElementException("Treet er tomt!"); med Objectes.requireNonNull(p); som sjekker den første veriden av p i postorden, og videre sjekker vi om p sin venster eller høyre ikke lik null, så returner vi p. jeg har løst oppgave 3 ved hjelp av kompediet, jeg har kopiert koden i kompediet 5.1.7h, men fikk feil når jeg testet oppgaven. Så byttet jeg if (tom()) throw new NoSuchElementException("Treet er tomt!"); med Objects.requireNonNull(p); som sjekker den første verdien av p i postorden. På nestePostorden vi skulle lage kode som skal returnere den noden som kommer etter p i postorden. Hvis p er den siste i postorden, skal metoden returnere null.

I oppgave 4 Jeg har implementet den første funksjonen uten av rekursjon og uten bruk av hjelpevariabler som stack / queue som står på obligen. Jeg har brukt funksjonen nestePostorden fra forrige oppgave, som start med å finne den første noden p i postorden. jeg har laget en while-løkke som lopper gjennom treet og oppdaterer neste verdi i postorden.

