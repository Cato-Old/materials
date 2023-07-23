## Ćwiczenie nr 1
Dane są dwie liczby całkowite. Zwróć ich iloczyn tylko jeżeli ich iloczyn jest mniejszy od 1000 w przeciwnym razie zwróć ich sumę
### Przykłady
#### Wejście nr 1
> `number1 = 20`
> `number2 = 30`
#### Wyjście nr 1
> `The result is 600`
#### Wyjście nr 2
> `number1 = 40`
> `number2 = 30`
#### Wyjście nr 2
> `The result is 70`
## Ćwiczenie nr 2
Napisz program, który doda pierwsze 10 liczb naturalnych i przy każdej operacji dodawania wypisze dodawane liczby i ich sumę.
### Przykład
#### Wyjście
> `Current number 0; Previous number 0; Sum: 0`
> `Current number 1; Previous number 0; Sum: 1`
> `Current number 2; Previous number 1; Sum: 3`
> `Current number 3; Previous number 2; Sum: 5`
> `Current number 4; Previous number 3; Sum: 7`
> `Current number 5; Previous number 4; Sum: 9` 
> `Current number 6; Previous number 5; Sum: 11`
> `Current number 7; Previous number 6; Sum: 13`
> `Current number 8; Previous number 7; Sum: 15`
> `Current number 9; Previous number 8; Sum: 17`
## Ćwiczenie nr 3
Napisz program, który przyjmie na wejściu od użytkownika string i wyświetla na wyjściu znaki, które są obecne na parzystych indeksach.
### Przykład
#### Wejście
> `Given string is: python`
#### Wyjście
> `p`
> `t`
> `o`
## Ćwiczenie nr 4
Napisz program, który dla podanej nazwy pliku wypisze rozszerzenie tego pliku.
### Przykład
#### Wejście
> `abc.java`
#### Wyjście
> `java`
## Ćwiczenie nr 5
Napisz program, który dla podanego stringa wypisze jego potrojoną kopię.
### Przykład
#### Wejście
> `abc`
#### Wyjście
> `abcabcabc`
## Ćwiczenie nr 6
Napisz program, który dla podanej liczby całkowitej wypisze czy jest ona parzysta czy nieparzysta.
### Przykład
#### Wejście nr 1
> 6
#### Wyjście nr 1
> Liczba 6 jest parzysta.
#### Wejście nr 2
> 17
#### Wyjście nr 2
> Liczba 17 nie jest parzysta.
## Ćwiczenie nr 7
Napisz funkcję, która przyjmie dowolną liczbę argumentów w postaci liczb całkowitych i zwróci ich sumę. Nie można użyć wbudowanej funkcji **sum**.
### Przykład
#### Wejście
> sum_up(1, 2, 3, 4, 5)
#### Wyjście
> 15
## Ćwiczenie nr 8
Napisz funkcję, która odwróci przekazany do niej string.
### Przykład
#### Wejście
> reverse_string("abcd1234")
#### Wyjście
> "4321dcba"
## Ćwiczenie nr 9
Napisz funkcję `show_employee`, która będzie przyjmowała dwa argumenty: obowiązkowy - nazwisko oraz opcjonalny - wynagrodzenie. Funkcja powinna zwrócić string, zawierający nazwisko pracownika oraz wynagrodzenie - o ile zostało podane, w przeciwnym wypadku wysokość wynagrodzenia powinna wynieść 9 000.
### Przykład
#### Wejście nr 1
> show_employee("Kowalski", 12000)
#### Wyjście nr 1
> Pracownik Kowalski zarabia 12000 zł
#### Wejście nr 2
> show_employee("Nowak")
#### Wyjście nr 2
> Pracownik Nowak zarabia 9000 zł
## Ćwiczenie nr 10
Napisz funkcję `parity_analisis`, która przyjmuje na wejściu liczbę całkowitą i zwraca `True` jeśli suma jej cyfr ma tę samą parzystość co dana liczba. W przeciwnym razie, zwraca `False`.
### Przykład
#### Wejście nr 1
> parity_analysis(243)
#### Wyjście nr 1
> True
> \# 243 jest nieparzyste i (2+4+3) = 9 jest nieparzyste -> True
#### Wejście nr 2
> parity_analisis(12)
#### Wyjście nr 2
> False
> \# 12 jest parzyste natomiast (1 + 2) = 3 jest nieparzyste -> False
#### Wejście nr 3
> parity_analisis(3)
#### Wyjście nr 3
> True
> \# 3 jest nieparzyste i 3 (suma cyfr) jest nieparzyste -> True
## Ćwiczenie nr 11
Napisz funkcję `binary`, która przyjmuje na wejściu reprezentację dziesiętną i zwraca binarną reprezentację tej liczby jako string. Reprezentacja binarna jest oparta na potęgach 2 - liczba dziesiętna 169 ma binarną reprezentacje 10101001(2) = 1 * 2^0 + 1 * 2^3 + 1 * 2^5 + 1 * 2^7 = 1 + 8 + 32 + 128 = 169.
### Przykład
#### Wejście nr 1
> binary(1)
#### Wyjście nr 1
> "1"
> \# 1 = 1 * 2^0
#### Wejście nr 2
> binary(5)
#### Wyjście nr 2
> "101"
> \# 5 = 1 * 2^2 + 1 * 2^0 = 4 + 1
#### Wejście nr 3
> binary(10)
#### Wyjście nr 
> "1010"
> \# 10 = 1 * 2^4 + 1 * 2^1 = 8 + 2 = 10
## Ćwiczenie nr 12
Napisz funkcję `flatten`, która przyjmuje na wejściu zagnieżdżoną listę i zwraca pojedynczą płaską listę, zawierającą wszystkie skalarne wartości oprócz `None`. Funkcja powinna przyjmować dowolnie głęboko zagnieżdżone listy lub tuple.
### Przykład
#### Wejście
> flatten([[1, 2, 3, null, 4], [null], 5])
#### Wyjście
> [1, 2, 3, 4, 5]
## Ćwiczenie 13
Stwórz funkcję, która na wejściu będzie przyjmowała liczbę całkowitą i zwróci `True` jeżeli liczba jest symetryczna oraz `False` jeżeli nie jest symetryczna. Liczba jest symetryczna, jeżeli po jej odwróceniu otrzymujemy tę samą liczbę.
### Przykład
#### Wejście nr 1
> is_symmetrical(7227)
#### Wyjście nr 1
> True
#### Wejście nr 2
> is_symmetrical(12567)
#### Wyjście nr 2
> False
#### Wejście nr 3
> is_symmetrical(444444444)
#### Wyjście nr 3
> True
#### Wejście nr 4
> is_symmetrical(1112111)
#### Wyjście nr 4
> True
## Ćwiczenie 14
Napisz program, który na wejściu będzie przyjmował listę liczb całkowitych oddzielonych spacjami, zweryfikuje ich poprawność i zwróci posortowaną listę w porządku rosnącym. W razie nieprawidłowych danych wejściowych zostanie wypisany komunikat: `Invalid input data: ` i nieprawidłowy element.
### Przykład
#### Wejście nr 1
> 5 1 2 4 6
#### Wyjście nr 1
> 1 2 4 5 6
#### Wejście nr 2
> 5 1 2 4 asdf
#### Wyjście nr 2
> Invalid input data: asdf
## Ćwiczenie 15
Dana jest lista zawierająca krotki z informacją o początku (pierwsza pozycja) i końcu wydarzenia (druga pozycja) w postaci liczb całkowitych. Napisz funkcję `sort_by_start`, która zwróci lisę krotek posortowaną w kolejności rosnącej według startów wydarzeń.
### Przykład
#### Wejście nr 1
> sort_by_start([(2, 3), (1, 4), (0, 10)])
#### Wyjście nr 1
> [(0, 10), (1, 4), (2, 3)]
## Ćwiczenie 16
Duża liczba całkowita jest reprezentowana poprzez listę jej cyfr. Napisz funkcję `add_one`, która zwróci taką samą reprezentację liczby po dodaniu do niej 1.
### Przykład
#### Wejście nr 1
> add_one([1, 2, 3])
#### Wyjście nr 1
> [1, 2, 4]
#### Wejście nr 2
> add_one([4, 3, 2, 1])
#### Wyjście nr 2
> [4, 3, 2, 2]
#### Wejście nr 3
> add_one([9])
#### Wyjście nr 3
> [1, 0]
