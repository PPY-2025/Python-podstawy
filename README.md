**Zadania dotyczące składni Pythona i podstaw programowania obiektowego**

---
### Zadanie 1: Podstawowe operacje w Pythonie
**Cel:** Poznanie podstawowej składni Pythona oraz operacji na zmiennych.

**Przykład:**  
```python
a = 10
b = 5.5
c = "Python"
print(a + b)
print(type(c))
```

**Zadanie:** 
1. Utwórz trzy zmienne: `x = 20`, `y = 7.3`, `z = "Nauka"`.
2. Wykonaj operacje matematyczne (+, -, *, /, //, %, **).
3. Sprawdź typ każdej zmiennej.
4. Wydrukuj wyniki.

---
### Zadanie 2: Instrukcje warunkowe
**Cel:** Nauka instrukcji warunkowych `if`, `elif`, `else`.

**Przykład:**  
```python
num = int(input("Podaj liczbę: "))
if num > 0:
    print("Liczba jest dodatnia.")
elif num < 0:
    print("Liczba jest ujemna.")
else:
    print("Liczba to zero.")
```

**Zadanie:** 
1. Pobierz liczbę od użytkownika.
2. Sprawdź, czy jest podzielna przez 3 i 5 jednocześnie.
3. Wydrukuj odpowiedni komunikat.

---
### Zadanie 3: Pętle `for` i `while`
**Cel:** Zapoznanie się z pętlami i ich zastosowaniem.

**Przykład:**  
```python
for i in range(1, 11):
    print(i)
```

**Zadanie:** 
1. Wypisz liczby od 1 do 50 za pomocą pętli `for`.
2. Utwórz pętlę `while`, która prosi użytkownika o wprowadzenie liczby większej niż 100.

---
### Zadanie 4: Listy w Pythonie
**Cel:** Poznanie list i operacji na nich.

**Przykład:**  
```python
lista = [1, 2, 3, 4, 5]
print(lista[0])
lista.append(6)
print(lista)
```

**Zadanie:** 
1. Stwórz listę zawierającą 5 ulubionych owoców.
2. Dodaj do niej nowy owoc i usuń pierwszy element.

---
### Zadanie 5: Słowniki w Pythonie
**Cel:** Praca ze słownikami.

**Przykład:**  
```python
slownik = {"imie": "Anna", "wiek": 25}
print(slownik["imie"])
```

**Zadanie:** 
1. Stwórz słownik zawierający trzy pary klucz-wartość opisujące książkę (np. tytuł, autor, rok wydania).
2. Wyświetl wartość klucza „autor”.

---
### Zadanie 6: Funkcje w Pythonie
**Cel:** Tworzenie i wywoływanie funkcji.

**Przykład:**  
```python
def suma(a, b):
    return a + b

print(suma(3, 5))
```

**Zadanie:** 
1. Napisz funkcję `mnoz(a, b)`, która zwróci iloczyn dwóch liczb.

---
### Zadanie 7: Programowanie obiektowe - klasy
**Cel:** Tworzenie klas i obiektów w Pythonie.

**Przykład:**  
```python
class Samochod:
    def __init__(self, marka, rok):
        self.marka = marka
        self.rok = rok
```

**Zadanie:** 
1. Stwórz klasę `Osoba` z polami `imie` i `wiek`.
2. Utwórz obiekt tej klasy i wydrukuj jego atrybuty.

---
### Zadanie 8: Dziedziczenie w Pythonie
**Cel:** Poznanie dziedziczenia.

**Przykład:**  
```python
class Pojazd:
    def __init__(self, marka):
        self.marka = marka
class Samochod(Pojazd):
    pass
```

**Zadanie:** 
1. Stwórz klasę `Zwierze` i dziedziczącą po niej klasę `Pies`.

---
### Zadanie 9: Obsługa wyjątków
**Cel:** Obsługa błędów.

**Przykład:**  
```python
try:
    x = int("test")
except ValueError:
    print("Błąd konwersji!")
```

**Zadanie:** 
1. Obsłuż wyjątek przy dzieleniu przez zero.

---
### Zadanie 10: Praca z plikami
**Cel:** Operacje na plikach.

**Przykład:**  
```python
with open("plik.txt", "w") as f:
    f.write("Witaj!")
```

**Zadanie:** 
1. Stwórz plik `dane.txt`, zapisz do niego kilka linijek tekstu i odczytaj jego zawartość.

---
### Zadanie 11: Moduły w Pythonie
**Cel:** Importowanie i używanie modułów.

**Przykład:**  
```python
import math
print(math.sqrt(16))
```

**Zadanie:** 
1. Zaimportuj moduł `random` i wygeneruj losową liczbę z przedziału od 1 do 100.

---
### Zadanie 12: Wyrażenia regularne
**Cel:** Wyszukiwanie wzorców w tekście.

**Przykład:**  
```python
import re
pattern = r"a.c"
text = "abc, axc, azc, a123c"
match = re.findall(pattern, text)
print(match)
```

**Zadanie:** 
1. Napisz program sprawdzający, czy podany przez użytkownika email jest poprawny (z użyciem `re`).

---
### Zadanie 13: Generatory
**Cel:** Tworzenie generatorów w Pythonie.

**Przykład:**  
```python
def generator():
    for i in range(3):
        yield i

for val in generator():
    print(val)
```

**Zadanie:** 
1. Napisz generator zwracający kolejne liczby parzyste.

---
### Zadanie 14: Funkcje lambda
**Cel:** Użycie funkcji anonimowych.

**Przykład:**  
```python
kwadrat = lambda x: x * x
print(kwadrat(5))
```

**Zadanie:** 
1. Stwórz funkcję lambda, która zwraca sumę dwóch liczb.

