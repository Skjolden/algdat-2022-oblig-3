# Obligatorisk oppgave 3 i Algoritmer og Datastrukturer

Denne oppgaven er en innlevering i Algoritmer og Datastrukturer. 
Oppgaven er levert av følgende student:
* Eivind Skjolden, S362087, s362087@oslomet.no


# Oppgavebeskrivelse

I oppgave 1 så gikk jeg frem ved å kopiere programkode 5.2.3 a) og legge
til forelder til noden dersom den ikke er rotnoden.

I oppgave 2 starter antallet på 0 og itererer gjennom treet til det evt
finnes riktig verdi. Om det finnes flere av samme verdi vil den ligge
videre ned i treet på høyrebarnets side av første gangen verdien oppstår.
Når vi når en bladnode vet vi at det ikke finnes flere av den verdien og
antall returneres.

I oppgave 3 førstePostorden følger vi treets venstreside til det ikke
lenger er mulig, om siste node på venstreside har et alenebarn i høyreside
ender vi opp i den noden. I nestePostorden sjekker vi først at noden ikke
er rotnoden. Hvis p er høyrebarnet til forelderen så er forelderen den neste.
Dersom p er venstrebarn uten at forelder har høyrebarn er forelder neste.
Dersom p er venstrebarn til forelder med høyrebarn så er neste node første 
i postorden hvor høyrebarnet brukes som rot.

I oppgave 4 postorden starter vi i noden førsteorden til treet og itererer 
gjennom treet med nestePostorden til vi når rotnoden.
postordenRecursive itererer gjennom treet rekursivt, kode tatt fra kompendiet.

I oppgave 5 serialize bruker vi kø til å gå gjennom nodene i nivå orden. Første
noden blir lagt til med venstre barnet og høyrebarnet etter seg. Deretter får
hver forelder fra topp-venstre til bunn-høyre lagt til sine barn før de fjernes fra
køen til køen er tom. deserialize lager et nytt tre og legger inn alle verdiene i 
arrayet før treet returneres.
