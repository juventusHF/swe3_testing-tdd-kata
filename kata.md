# Stringbasierter Taschenrechner

Bitte die Aufgaben nicht zu weit im Vorraus lesen.

Vorgehensweise:
- nur eine Anforderung auf einmal entwickeln
- mit dem einfachsten Test für diese Anforderung anfangen
- den einfachsten Code schreiben, der den Test grün macht
- Input-Validierung / Fehlerbehandlung kann weggelassen werden
- Refactoring nicht vergessen

## Level 1

Anforderungen:
- `Calculator` Klasse im Package `ch.juventus.katas`
- `add`-Methode nimmt Strings entgegen nehmen und liefert eine ganze Zahl
- bei einem Leerstring oder null als Argument liefert die Methode 0.
- für 1 oder 2 Komma-separierte Zahlen liefert die Methode die Summe beider Zahlen,
  - z.B. `1,2` = 3

## Level 2

Anforderungen:
- Die Methode kann beliebig viele komma-separierte Zahlen entgegennehmen.
- Negative Zahlen führen zu einer `IllegalArgumentException`
  - alle negativen Zahlen sollen in der Exception gesammelt werden

## Level 3

Anforderungen:
- Die Methode akzeptiert neben Kommas auch Newlines ('\n') zur Separierung der Zahlen.
  - z.B. `1\n2,3` = 6
- Alle Zahlen grösser als 1000 sollen ignoriert werden.

## Level 4

Anforderungen:
- Eine optionale erste Zeile bestimmt den Delimiter mit folgendem Format: `//[delimiter]\n`
  - z.B. `//*\n1*2` = 3
