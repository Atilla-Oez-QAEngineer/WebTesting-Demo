# Bug Report – Lange Adresse wird im Output nicht sauber angezeigt

**ID:** BR-01  
**Zugehöriger Testfall:** TC05 – Lange Adresse (300 Zeichen)  
**Bereich:** DemoQA Text Box  
**Schweregrad:** Minor  
**Priorität:** Low  

## Beschreibung
Wenn in einem Adressfeld (z. B. "Current Address") eine sehr lange Eingabe gemacht wird (ca. 300+ Zeichen), wird der Text im Output-Bereich nicht sauber bzw. nicht vollständig angezeigt.

## Schritte zur Reproduktion
1. Öffne https://demoqa.com/text-box  
2. Gib in das Feld **"Current Address"** eine sehr lange Zeichenkette (ca. 300–500 Zeichen) ein  
3. Lass die anderen Felder normal oder leer  
4. Klicke auf **Submit**  
5. Beobachte den Output-Bereich unter dem Formular

## Erwartetes Ergebnis
Die komplette Adresse sollte im Output-Bereich vollständig und lesbar angezeigt werden.

## Tatsächliches Ergebnis
Der Text wird im Output-Bereich optisch nicht sauber dargestellt (überlappend).

## Screenshot
[Screenshot
](https://github.com/Atilla-Oez-QAEngineer/WebTesting-Demo/blob/a47445e4c39b6d00c65851a44312211c81303b53/Screenshots/TC05-long-address-output.png)
