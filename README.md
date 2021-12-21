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
 
Dodatkowo w przypadku `Worrior`'a gdy blokuje cios używa `shield` która blokuje `shieldPenetration` % obrażeń od ciosu przeciwnika.
`Hunter` ma umiejętność `dodge` , która daje mu % szans na uniknięcie otrzymania obrażeń od ciosu.
`Mage` nie posiada żadnych umiejętnosci tego typu :(

### Statystyki

Postać posiada kolejno:
`hp` - ilość "krwinek"
`xp` - ilość doświadczenia
`endurence` - wytrzymałość postaci, 1pkt wytrzymałości daje:
  - 10pkt do `hp` dla `Warriora`
  - 7pkt do `hp` dla `Huntera`
  - 5pkt do `hp` dla `Mage`
 
