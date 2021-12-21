# Heros-battler
Projekt 2 OP

## Ogólny opis
Autobattler stworzonych przez użytkownika postaci, które mogą posiadać różne klasy postaci oraz statystyki.

## Cel gry 
Cel gry jest w sumie bliżej nieokreślony bo zakładając, że nie będzie max lvl postaci w grę można grać właściwie bez końca.

## Co powinien mieć nasz bohater ?

### Klasy
Każdy bohater ma jedną z 3 klas:
- `Mage`
- `Worrior`
- `Hunter`
Każda z tych klas ma swoją unikalną broń, kolejno:
- `MageStaff`
- `Sword`
- `Bow`
 
Dodatkowo w przypadku `Worrior`'a gdy blokuje cios używa `shield` która blokuje `shieldProtection` % obrażeń od ciosu przeciwnika (max 50%).
`Hunter` ma umiejętność `dodge`  (max 50%) , która daje mu % szans na uniknięcie otrzymania obrażeń od ciosu.
`Mage` nie posiada żadnych umiejętnosci tego typu :(

### Statystyki

Postać posiada kolejno:
`hp` - ilość "krwinek"
`xp` - ilość doświadczenia
`dmg` - obrażenia zadawane
`endurence` - wytrzymałość postaci, 1pkt wytrzymałości daje:
  - 10pkt do `hp` dla `Warriora`
  - 7pkt do `hp` dla `Huntera`
  - 5pkt do `hp` dla `Mage`
 
 `strength` - siła postaci, 1pkt siły daje:
 - każdemu daje 1pkt do odporności przeciwko `Warrior`
 - `Warrior` dostaje za 1pkt siły +10pkt do `dmg`
 
 `dexterity` - zręcznośc postaci, 1pkt zręczności daje:
 - każdemu daje 1pkt do odporności przeciwko `Hunter`
 - `Hunter` dostaje za 1pkt siły +12pkt do `dmg` oraz + 1% do `dodge` (max 50%)
 
 `intelligence` - inteligencja postaci, 1pkt inteligencji daje:
  - każdemu daje 1pkt do odporności przeciwko `Mage`
 - `Mage` dostaje za 1pkt inteligencji +20pkt do `dmg`
 
 `luck` - dla każdej postaci każdy pkt szczęścia dodaje 1% `dmg` przy ataku, (max 100pkt) [więcej w sekcji walka]
 
 ### Walka
 - Walka przebiega turowo, postać atakująca pierwsza jest losowana.
 - Mamy dwóch wojowników `heroA` i `heroB` , załóżmy, że `heroA` zaczyna
 - Poniższy cykl powtarza się, aż do "stracenia przytomności" jednego z nich
  - `heroA` atakuje 
   - atakując za dmg pomiędzy `0` a `heroA.dmg*(100+heroA.luck)` 
  - `heroB` używa:
  1. `block` jeśli jego klasa to `Warrior`:
   - blokuje `shieldProtection`
  2. 
  - , `dodge` jeśli klasa to `Hunter` lub nic nie robi jeśli `Mage`
  - `heroB` atakuje
  - `heroA` używa `block` jeśli jego klasa to `Warrior`, `dodge` jeśli klasa to `Hunter` lub nic nie robi jeśli `Mage`
 
 
 
 
 
