# Testfälle – DemoQA Text Box

Getestete Seite: https://demoqa.com/text-box  
Testdatum: 04.12.2025

---

## TC01 – Gültigen vollständigen Namen eingeben
**Vorbedingungen:** Seite ist geöffnet  
**Testschritte:**  
1. „Atilla Test“ in das Feld „Full Name“ eingeben  
2. Auf „Submit“ klicken  
**Erwartetes Ergebnis:** Name erscheint korrekt im Output-Bereich.  
**Ist-Ergebnis:** Name wird korrekt angezeigt.  
**Status:** PASS

---

## TC02 – Full Name leer lassen
**Vorbedingungen:** Seite geöffnet  
**Testschritte:**  
1. „Full Name“ leer lassen  
2. Submit klicken  
**Erwartetes Ergebnis:** Output zeigt keinen Namen an.  
**Ist-Ergebnis:** Kein Name wird angezeigt.  
**Status:** PASS

---

## TC03 – Ungültige Email eingeben
**Vorbedingungen:** Seite geöffnet  
**Testschritte:**  
1. „test123“ in das Emailfeld eingeben  
2. Submit klicken  
**Erwartetes Ergebnis:** Emailfeld wird rot markiert.  
**Ist-Ergebnis:** Emailfeld wird rot markiert.  
**Status:** PASS

---

## TC04 – Gültige Email eingeben
**Vorbedingungen:** Seite geöffnet  
**Testschritte:**  
1. „test@mail.com“ eingeben  
2. Submit  
**Erwartetes Ergebnis:** Email wird korrekt angezeigt.  
**Ist-Ergebnis:** Email wird korrekt angezeigt.  
**Status:** PASS

---

## TC05 – Lange Adresse (300 Zeichen) eingeben
**Vorbedingungen:** Seite geöffnet  
**Testschritte:**  
1. 300 Zeichen in „Current Address“ eingeben  
2. Submit  
**Erwartetes Ergebnis:** Adresse wird vollständig angezeigt.  
**Ist-Ergebnis:** Anzeige ist fehlerhaft / nicht sauber (siehe Bugreport BR-01).  
**Status:** FAIL

---

## TC06 – Current Address leer lassen
**Vorbedingungen:** Seite geöffnet  
**Testschritte:**  
1. Feld leer lassen  
2. Submit  
**Erwartetes Ergebnis:** Keine Adresse wird angezeigt.  
**Ist-Ergebnis:** Keine Adresse wird angezeigt.  
**Status:** PASS

---

## TC07 – Submit ohne Eingaben
**Vorbedingungen:** Seite geöffnet  
**Testschritte:**  
1. Alle Felder leer lassen  
2. Submit  
**Erwartetes Ergebnis:** Output zeigt leere Werte.  
**Ist-Ergebnis:** Output zeigt leere Werte.  
**Status:** PASS

---

## TC08 – Current Address & Permanent Address gleich setzen
**Vorbedingungen:** Seite geöffnet  
**Testschritte:**  
1. „Hallo Welt“ in Current Address  
2. „Hallo Welt“ in Permanent Address  
3. Submit  
**Erwartetes Ergebnis:** Beide Adressen erscheinen identisch.  
**Ist-Ergebnis:** Beide Adressen erscheinen identisch.  
**Status:** PASS

---

## TC09 – Sonderzeichen im Namen
**Vorbedingungen:** Seite geöffnet  
**Testschritte:**  
1. „Atilla @#!“ eingeben  
2. Submit  
**Erwartetes Ergebnis:** System akzeptiert Eingabe.  
**Ist-Ergebnis:** System akzeptiert Eingabe.  
**Status:** PASS

---

## TC10 – Extrem lange Eingaben in allen Feldern
**Vorbedingungen:** Seite geöffnet  
**Testschritte:**  
1. In alle Felder 300–500 Zeichen eingeben  
2. Submit  
**Erwartetes Ergebnis:** Formular verarbeitet alles ohne Probleme.  
**Ist-Ergebnis:** Seite friert ein / Browser meldet „Diese Seite antwortet nicht“ (siehe Bugreport BR-02).  
**Status:** FAIL
