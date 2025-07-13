# Python Grundlagen - Übungsaufgaben

## Aufgaben Teil 1: Literale und Bezeichner

### Aufgabe 1: Literale in Python
Diese Aufgabe demonstriert die verschiedenen Arten von Literalen in Python:

- **Ganzzahl (int)**: `anzahl_kinder = 3`
- **Gleitkommazahl (float)**: `durchschnittsnote = 2.7`
- **Zeichenfolge (str)**: `willkommensnachricht = "Willkommen zu meinem ersten Python-Projekt!"`
- **Boolean (bool)**: `ist_aktiv = True`
- **Liste (list)**: `wochentage = ["Montag", "Dienstag", "Mittwoch", "Donnerstag", "Freitag"]`

### Aufgabe 2: Bezeichner und Kommentare
Die Bezeichner wurden sinnvoll gewählt und mit Kommentaren versehen, die ihren Zweck erklären.

## Teil 2: Namensräume

### Aufgabe 3: Lokale und globale Variablen
Demonstriert den Unterschied zwischen lokalen und globalen Variablen:

```python
benutzername = "MaxMustermann"  # Globale Variable

def zeige_namensraeume():
    benutzername = "LokalMax"  # Lokale Variable
    print("Lokale Variable:", benutzername)
    print("Globale Variable:", globals()["benutzername"])
```

### Aufgabe 4: Verschachtelte Namensräume
Zeigt die Verwendung von `nonlocal` zur Änderung von Variablen in äußeren Namensräumen:

```python
def aussen():
    variable = "Ursprünglicher Wert"
    
    def innen():
        nonlocal variable
        variable = "Geänderter Wert"
    
    innen()
    print("Variable nach Änderung:", variable)
```

## Teil 3: Built-in Funktionen

### Aufgabe 5: Wichtige Built-in Funktionen
Demonstriert verschiedene nützliche Built-in Funktionen:

```python
zahlen_liste = [3, 7, 1, 9, 5]
print("Länge der Liste:", len(zahlen_liste))
print("Typ der Liste:", type(zahlen_liste))
print("Summe der Liste:", sum(zahlen_liste))
print("Maximale Zahl:", max(zahlen_liste))
print("Minimale Zahl:", min(zahlen_liste))
print("Sortierte Liste:", sorted(zahlen_liste))
```

### Aufgabe 6: Eingaben verarbeiten
Zeigt, wie Benutzereingaben verarbeitet und validiert werden:

```python
eingabe = input("Bitte geben Sie eine Zahl ein: ")

try:
    zahl = int(eingabe)
    if isinstance(zahl, int):
        print(f"Die eingegebene Zahl ist: {zahl}")
except ValueError:
    print("Die Eingabe ist keine gültige Zahl.")
```

## Anleitung zur Ausführung

1. Speichern Sie den Code in einer Datei namens `Aufgaben_1.py`
2. Führen Sie die Datei mit Python aus:
   ```
   python Aufgaben_1.py
   ```
3. Folgen Sie den Anweisungen im Programm

## Lernziele

- Verständnis der verschiedenen Datentypen in Python
- Unterschied zwischen lokalen und globalen Variablen
- Umgang mit Namensräumen und Scope
- Anwendung wichtiger Built-in Funktionen
- Verarbeitung von Benutzereingaben

## Lizenz
Dieses Projekt steht unter der MIT-Lizenz.
