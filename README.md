# Web-Workshop React Teszt

A projekt csak egy üres create-react-app-s template, amiben már előre vannak telepítve a feladat elvégzéhes szükséges package-k. A feladat leírása bekezdésben van pontosan leírva, hogy mit kell implementálni.

A project **^18 vagy a feletti node verzióval** lehet elindítani és yarn package managert használ. Remélem mindenkénel telepítve van a  **nvm** (node version manager), ha mégsem akkor telepítsétek. Ellenőrizzétek le hogy jó node verziót használtok (`nvm list`, `nvm use [verzió szám]`).  Pullolás után adjátok ki a `yarn install` parancsot a projekt mappában, majd el tudjátok indítani a `yarn run start` paranccsal.

## Feladat leírása

1. Hozz létre egy form-t (react-hook-form-l), ami a egy felhasználó adatait kéri be:
- Név (max. 50 karakteres és nem tartalmazhat számokat)
- Életkor (1-100 közötti egészszámnak kell lennie)
- Email (valid email címnek kell hogy legyen)
- Jelszó (minimum 6 karakteres legyen és tartalmazzon számot legalább 1 számot)
- Jelszó megerősítés (meg kell hogy eggyezzen a 'Jelszó' field-ben lévő értékkel)

Ezeket az értékeket validálni kell valamilyen resolver-l és ha hiba van valamelyik fieldben, akkor a filed alatt írja ki pirossal hogy pontosan mi a hiba. Majd ezeket az értékeket (a Jelszó megerősítés field nélkül) mentsd el redux-ba.

2. Hozz létre egy redux slice-t amivel a state-be el tudod menteni a felhasználók adatait. Ennek egy listának kell lennie. A reduxba csak akkor mentse el a felhasználót ha az 1.s pontban feltételeknek megfelel valamint ha még nem létezik olyan nevű felhasználó.

3. Hozz létre egy olyan redux selectort, ami egy **listában** visszaadja ezt a formázott **stringet** felhasználónként: `'Szia, {felhasználónév} ({kor}) - {email} !'`. Majd ezeket a stringeket jelenítsd meg a form alatt valahogy listázva listázva.

A feladatokat csakk akkor lehet elfogadni, a console-ban se hiba se warn nincs!

Stílus és kinézet nem fontos, persze ha van idő akkor lehet plusz pont ha styled-componenteket hoztok létre.

A kész feladatokat node_modules mappa nélkül tötlsétek fel saját github-ra vagy küldjétek el nekem .zip / .rar-ban.