# Bug Report – Seite reagiert nicht bei sehr langen Eingaben in allen Feldern

**ID:** BR-02  
**Zugehöriger Testfall:** TC10 – Extrem lange Eingaben in allen Feldern  
**Bereich:** DemoQA Text Box  
**Schweregrad:** Major  
**Priorität:** Medium  

## Beschreibung
Wenn in **allen Feldern** (Full Name, Email, Current Address, Permanent Address) sehr lange Texte eingegeben werden (300+ Zeichen), reagiert die Seite teilweise nicht mehr. Der Browser zeigt die Meldung „Diese Seite antwortet nicht“.

## Schritte zur Reproduktion
1. Öffne https://demoqa.com/text-box  
2. Gib in **alle Felder** (Full Name, Email, Current Address, Permanent Address) jeweils eine sehr lange Zeichenkette (ca. 300–500 Zeichen) ein  
3. Klicke auf **Submit**  
4. Beobachte das Verhalten des Browsers

## Erwartetes Ergebnis
Die Seite sollte die Eingaben stabil verarbeiten, das Formular absenden und den Output anzeigen, ohne dass die Seite einfriert.

## Tatsächliches Ergebnis
Die Seite hängt / reagiert nicht mehr und der Browser zeigt ein Pop-up wie „Diese Seite antwortet nicht“ (z. B. in Chrome).

## Screenshot
[(Screenshot von der Fehlermeldung im Ordner `Screenshots/` speichern und hier referenzieren.)](https://github.com/Atilla-Oez-QAEngineer/WebTesting-Demo/blob/b38f10a913188d713f812e3af058ff887ab69e3c/Screenshots/TC10-page-freeze.png)
