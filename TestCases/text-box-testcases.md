# Testfälle – DemoQA Text Box

Getestete Seite: https://demoqa.com/text-box  
Dieses Dokument enthält 10 grundlegende Testfälle für das Text Box Formular.

---

## TC01 – Gültigen vollständigen Namen eingeben
**Vorbedingungen:** Seite ist geöffnet  
**Testschritte:**  
1. „Atilla Test“ in das Feld „Full Name“ eingeben  
2. Auf „Submit“ klicken  
**Erwartetes Ergebnis:**  
Der Name erscheint korrekt im Output-Bereich.

---

## TC02 – Full Name leer lassen
**Vorbedingungen:** Seite ist geöffnet  
**Testschritte:**  
1. „Full Name“ leer lassen  
2. Submit klicken  
**Erwartetes Ergebnis:**  
Output zeigt keinen Namen an (oder Feld bleibt leer).

---

## TC03 – Ungültige Email eingeben
**Vorbedingungen:** Seite ist geöffnet  
**Testschritte:**  
1. „test123“ in das Feld „Email“ eingeben  
2. Submit klicken  
**Erwartetes Ergebnis:**  
Das Emailfeld wird rot markiert (Fehlermarkierung).

---

## TC04 – Gültige Email eingeben
**Vorbedingungen:** Seite ist geöffnet  
**Testschritte:**  
1. „test@mail.com“ in das Email-Feld eintragen  
2. Submit klicken  
**Erwartetes Ergebnis:**  
Die Email erscheint korrekt im Output-Bereich.

---

## TC05 – Lange Adresse (300 Zeichen) eingeben
**Vorbedingungen:** Seite ist geöffnet  
**Testschritte:**  
1. 300 Zeichen in „Current Address“ eintragen  
2. Submit klicken  
**Erwartetes Ergebnis:**  
Die Adresse wird vollständig im Output angezeigt.

---

## TC06 – Current Address leer lassen
**Vorbedingungen:** Seite ist geöffnet  
**Testschritte:**  
1. Feld „Current Address“ leer lassen  
2. Submit  
**Erwartetes Ergebnis:**  
Keine Adresse wird im Output angezeigt.

---

## TC07 – Submit ohne Eingaben
**Vorbedingungen:** Seite ist geöffnet  
**Testschritte:**  
1. Alle Felder leer lassen  
2. Submit klicken  
**Erwartetes Ergebnis:**  
Output zeigt alle Felder leer an.

---

## TC08 – Current Address & Permanent Address gleich setzen
**Vorbedingungen:** Seite ist geöffnet  
**Testschritte:**  
1. „Hallo Welt“ in Current Address eintragen  
2. „Hallo Welt“ in Permanent Address eintragen  
3. Submit  
**Erwartetes Ergebnis:**  
Beide Adressen erscheinen identisch im Output.

---

## TC09 – Sonderzeichen im Namen
**Vorbedingungen:** Seite ist geöffnet  
**Testschritte:**  
1. „Atilla @#!“ eingeben  
2. Submit  
**Erwartetes Ergebnis:**  
System akzeptiert Eingabe oder zeigt ggf. Validierung an.

---

## TC10 – Extrem lange Eingaben in allen Feldern
**Vorbedingungen:** Seite ist geöffnet  
**Testschritte:**  
1. In alle Felder 300–500 Zeichen eingeben  
2. Submit  
**Erwartetes Ergebnis:**  
Formular verarbeitet alle Eingaben ohne Absturz, Output zeigt Daten.

