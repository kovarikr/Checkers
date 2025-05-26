# Konzolová Dáma (Checkers in C#)

Jednoduchá konzolová implementace hry **dáma** (checkers) pro dva hráče. Projekt je napsán v jazyce **C#** a běží v příkazové řádce (Console App).

## 🎮 Popis hry

- Hra je určena pro dva hráče hrající na jednom počítači.
- Každý hráč hraje střídavě, přičemž jeho cílem je **odstranit všechny soupeřovy figurky**.
- Figurka se může pohybovat **diagonálně** vpřed (nebo oběma směry, pokud je z ní král).
- Při přeskočení soupeřovy figurky je tato odstraněna.

## ♟️ Značky figurek:

- `O` – Hráč 1 (obyčejná figurka)
- `K` – Hráč 1 (král)
- `X` – Hráč 2 (obyčejná figurka)
- `Q` – Hráč 2 (král)
- `-` – Prázdné pole

## ▶️ Spuštění

1. Otevřete projekt v libovolném IDE pro C# (např. Visual Studio nebo Rider).
2. Zkompilujte a spusťte projekt jako konzolovou aplikaci.

Alternativně spusťte přeložený `.exe` soubor v příkazové řádce:
```bash
dotnet run
```

## 🕹️ Ovládání

Hra běží v konzoli a hráči zadávají své tahy ručně pomocí souřadnic.

Souřadnice se zadávají ve formátu: řádek sloupec (odděleno mezerou).

Nejprve zadáte startovní pozici figurky a poté cílovou pozici.

Příklad tahu:
java
Zkopírovat
Upravit
Vložte začínající řádek a sloupec (oddělit mezerou):
2 0
Vložte končící řádek a sloupec (oddělit mezerou):
3 1
Pokud je tah neplatný, zobrazí se hláška a hráč musí zadat nový tah.

Při dosažení poslední řady se obyčejná figurka promění na krále (K nebo Q).

## ⚠️ Omezení
Neimplementuje vícenásobné skákání (multi-jumps).

Neřeší automaticky tahy krále diagonálně dozadu (chování krále je částečně nedokončené).

Ošetření vstupu je základní – uživatel musí zadávat korektní čísla mezi 0–7.

## 📁 Struktura
Program.cs – hlavní soubor s logikou hry

Všechny metody (IsValidMove, Vyhral, VykresliPole) jsou definovány ve stejné třídě

## 🛠️ Možnosti vylepšení
Přidat AI protihráče

Vylepšit pravidla (např. vícenásobné skoky, nucené skákání)

Přidat grafické uživatelské rozhraní (GUI) pomocí WinForms nebo WPF

Implementovat ukládání a načítání stavu hry

