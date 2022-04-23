# Szoftvertervezés házifeladat


# TODO

US el van írva.

Primary actor

Részletes leírás aktorra vonatkozik nem a felhasználóra így ezt ki kell cserélni a rászoruló menekültre.

Egyik ágat érdemes lett volna szétszedni hogy főágba szedni.

mi történik a felületene,





## Csapattagok - bbm
- Krisztik Bálint
- Mihalik Márk
- Vezse Botond

## Feladatkiírás

**9. Élelmiszer, ill. étkezési lehetőség keresése a felajánlott támogatások között.**

## Aktorok

Rászoruló menekült: Az az ukrán menekült, aki igénybe kívánja venni a rendszeres étkezési segélycsomagot.

## Use case-ek

### US1: Menekült bejelentkeztetése

#### Aktor: 
Rászoruló menekült

#### Rövid leírás: 
A már regisztrált rászoruló menekült megadja a regisztrációkor megadott felhasználó nevét és jelszavát. Ezután hozzáfér a rendszer szolgáltatásaihoz.

### US2: Élelmiszerellátás és felajánlások keresése

#### Aktor: 
Rászoruló menekült

#### Rövid leírás:
A már bejelentkezett felhasználó a rendszerben eltárolt élelmiszer felajánlások és étkezési lehetőségek között kereshet és megtekintheti annak a részleteit.

#### Részletes leírás:

1. A felhasználó elindítja az élelmiszer ellátási szolgáltatások közötti keresést
2. Bejelölheti a felhasználó, hogy: (ide az kell h a rednszer megjelenítui)
    - rendszeres étkeztetést, 
    - vagy egyszeri tartós élelmiszer csomagot szeretne választani.
    Abban az esetben, ha az egyszeri tartós élelmiszert választja, akkor a folyamat az `5.` pontnál folytatódik.
3. Amennyiben a rendszeres étkeztetést választja a felhasználó, akkor az alábbiak közül választhat: (a felhasználó kiválasztja)(ki kell jelölni hogy elágazik és ha oda ágazik akkor ezt jelenítni meg és stb.) a menekült liválaszt
    - reggeli,
    - ebéd,
    - vacsora.
4. Ezek után a felhasználó kiválaszthatja az étkeztetés jellegét is, hogy: (a menekült kiválasztja majd a rednszer megjeleníti hogy milyen opciót választhat.) 
(Ügyesen ki kell találni a felhasználói felületet, mert az így nem annyira eldönthető nem jól specifikált?!)
    - hideg,
    - vagy meleg étkezést kíván igénybe venni.

5. Opcionálisan a felhasználó legördülő listákból kiválaszthatja, hogy hol szeretné igénybe venni vagy átvenni a felajánlást megyére, városra vagy városrészre lebontva. 
Le kell írni hogy ha előbb mit választott akkor a rendszer lekördülő alapján meghatározza mit kell megjelenni és megjeleníti az eredményeket, majd a felhasználó kiválasztja ami kell neki.
6. Opcionálisan a felhasználó kiválaszthatja, hogy mely napokon szeretné a rendszeres étkeztetést igénybe venni vagy melyik nap szeretné átvenni az egyszeri élelmiszer csomagot.

7. Amennyiben a rendszer hozott találatot a felhasználó által megadott feltételek mellett, akkor az így létrejött listából kiválaszthatja a számára legmegfelelőbb ajánlatot. Amennyiben nincs találat vagy a felhasználó módosítani szeretné a keresési feltételeket, akkor visszadobja a `2.` ponthoz.
8. Az ajánlat kiválasztása után a felhasználónak megjelennek a felajánló elérhetőségei. 