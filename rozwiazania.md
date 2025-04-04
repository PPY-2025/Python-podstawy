## Szczegółowy opis zadań z README.md z rozwiązaniami i wyjaśnieniami

---
### Zadanie 1: Podstawowe operacje w Pythonie
**Cel:** Nauka operacji matematycznych oraz typów danych.

**Opis i rozszerzenia:**
- Użyj zmiennych `x = 20`, `y = 7.3`, `z = "Nauka"`.
- Wykonaj wszystkie podstawowe operacje matematyczne z `x` i `y`.
- Uwzględnij możliwość błędów (np. dzielenie przez zero) za pomocą `try-except`.
- Iteruj po liście operacji, co pozwala uprościć kod i ułatwia jego rozbudowę.

**Kod:**
```python
x = 20
y = 7.3
z = "Nauka"

operacje = [
    ("Dodawanie", lambda a, b: a + b),
    ("Odejmowanie", lambda a, b: a - b),
    ("Mnożenie", lambda a, b: a * b),
    ("Dzielenie", lambda a, b: a / b),
    ("Modulo", lambda a, b: a % b),
    ("Potęgowanie", lambda a, b: a ** b)
]

for nazwa, operacja in operacje:
    try:
        print(f"{nazwa}: {operacja(x, y)}")
    except Exception as e:
        print(f"{nazwa}: Błąd - {e}")

for zmienna in [x, y, z]:
    print(f"Typ zmiennej {zmienna}: {type(zmienna)}")
```

---
### Zadanie 2: Instrukcje warunkowe
**Cel:** Nauka logicznych warunków.

**Opis:**
- Pobieramy liczbę od użytkownika.
- Sprawdzamy, czy liczba jest podzielna jednocześnie przez 3 **i** 5 (operator `and`).

**Kod:**
```python
try:
    liczba = int(input("Podaj liczbę: "))
    if liczba % 3 == 0 and liczba % 5 == 0:
        print("Liczba jest podzielna przez 3 i 5.")
    else:
        print("Liczba NIE jest podzielna przez 3 i 5.")
except ValueError:
    print("Nieprawidłowa wartość. Podaj liczbę całkowitą.")
```

---
### Zadanie 3: Pętle `for` i `while`
**Cel:** Nauka iteracji.

**Opis:**
1. Użycie pętli `for` do wypisania liczb od 1 do 50.
2. Pętla `while`, która wymusza podanie liczby > 100.

**Dlaczego lepiej sprawdzać zbór niż jego dopełnienie?**
Lepiej sprawdzać warunek pozytywny (zbór poprawnych wartości), np. `if liczba > 100`, ponieważ:
- Jest bardziej czytelny i logiczny.
- Unikamy złożony zaprzeczeń, np. `not liczba <= 100`.
- Łatwiej definiować i testować poprawne przypadki.

**Kod:**
```python
# for
for i in range(1, 51):
    print(i, end=" ")

# while
while True:
    try:
        liczba = int(input("\nPodaj liczbę większą niż 100: "))
        if liczba > 100:
            print("Dziękuję!")
            break
        else:
            print("Za mała liczba. Spróbuj ponownie.")
    except ValueError:
        print("To nie jest poprawna liczba.")
```

---
### Zadanie 4: Listy
**Cel:** Poznanie podstaw operacji na listach.

**Kod:**
```python
owoce = ["jabłko", "banan", "gruszka", "truskawka", "arbuz"]
owoce.append("kiwi")
del owoce[0]
print(owoce)
```

---
### Zadanie 5: Słowniki
**Cel:** Używanie par klucz-wartość.

**Kod:**
```python
ksiazka = {"tytul": "Wiedźmin", "autor": "Sapkowski", "rok": 1993}
print("Autor:", ksiazka["autor"])
```

---
### Zadanie 6: Funkcje
**Cel:** Definiowanie własnych funkcji.

**Kod:**
```python
def mnoz(a, b):
    return a * b

print(mnoz(3, 4))
```

---
### Zadanie 7: Klasy i obiekty
**Cel:** Podstawy OOP.

**Kod:**
```python
class Osoba:
    def __init__(self, imie, wiek):
        self.imie = imie
        self.wiek = wiek

os = Osoba("Anna", 30)
print(os.imie, os.wiek)
```

---
### Zadanie 8: Dziedziczenie
**Cel:** Zrozumienie dziedziczenia klas.

**Kod:**
```python
class Zwierze:
    def __init__(self, gatunek):
        self.gatunek = gatunek

class Pies(Zwierze):
    def szczekaj(self):
        print("Hau hau!")

p = Pies("ssak")
p.szczekaj()
```

---
### Zadanie 9: Obsługa wyjątków
**Kod:**
```python
try:
    a = int(input("Podaj licznik: "))
    b = int(input("Podaj mianownik: "))
    print(a / b)
except ZeroDivisionError:
    print("Błąd: dzielenie przez zero!")
except ValueError:
    print("Nieprawidłowe dane wejściowe.")
```

---
### Zadanie 10: Pliki
**Kod:**
```python
with open("dane.txt", "w") as f:
    f.write("Linia 1\nLinia 2\nLinia 3")

with open("dane.txt", "r") as f:
    print(f.read())
```

---
### Zadanie 11: Moduły
**Kod:**
```python
import random
print(random.randint(1, 100))
```

---
### Zadanie 12: Wyrażenia regularne
**Kod:**
```python
import re
email = input("Podaj email: ")
if re.match(r"^[\w\.-]+@[\w\.-]+\.\w+$", email):
    print("Email poprawny")
else:
    print("Niepoprawny email")
```

---
### Zadanie 13: Generatory
**Kod:**
```python
def parzyste():
    i = 0
    while True:
        yield i
        i += 2

for i, liczba in enumerate(parzyste()):
    if i == 5:
        break
    print(liczba)
```

---
### Zadanie 14: Lambda
**Kod:**
```python
suma = lambda a, b: a + b
print(suma(3, 5))
```
