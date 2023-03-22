# Tworzenie środowiska (Windows)
## Instalacja Pythona
1. Ze strony [python.org](https://www.python.org/downloads/release/python-3111/) pobieramy odpowiedni instalator Pythona w wersji 3.11. Najczęściej właściwym wyborem będzie `Windows installer (64-bit)` .
2. Instalujemy Pythona w systemie.
3. Wchodzimy do konsoli (skrót `WIN+R` i wpisujemy `cmd.exe` - aby uruchomić w trybie administratora naciskamy `CTRL+SHIFT+ENTER`) i wpisujemy `python --version`. Jeżeli uzyskamy komunikat: `Python 3.11.0` lub podobny (chodzi o wersję 3.11 Pythona) to możemy przejść do konfigurowania pip. W innym wypadku kontynuujemy wykonywanie tej instrukcji.
4. Ustalamy ścieżkę do naszej instalacji. Najprawdopodobniej będzie to coś podobnego do `C:\Users\<nazwa użytkownika>\AppData\Local\Programs\Python\Python311`, ale dla pewności warto prześledzić dokąd prowadzą linki z menu Start.
5. Uruchamiamy ustawianie zmiennych środowiskowych (w konsoli cmd wpisujemy `rundll32.exe sysdm.cpl,EditEnvironmentVariables`)
6. W górnym okienku wybieramy zmienną `Path` i klikamy edytuj.
7. Upewniamy się, że wśród ścieżek podanych w tej zmiennej ścieżka do instalacji Pythona 3.11 znajduje się na samej górze, jeśli nie to dodajemy ją i umieszczamy tam.
8. Powtarzamy punkty 6. i 7. dla dolnego okienka.
9. Po zamknięciu edytora zmiennych środowiskowych restartujemy konsolę cmd i jeszcze raz wpisujemy polecenie `python --version`. Jeżeli wszystko wykonaliśmy poprawnie, powinniśmy uzyskamy komunikat: `Python 3.11.0` lub podobny.
## Ustawienie pip
1. Wchodzimy do konsoli cmd (skrót `WIN+R` i wpisujemy `cmd.exe` - aby uruchomić w trybie administratora naciskamy `CTRL+SHIFT+ENTER`) i wpisujemy `pip --version`. Powinniśmy uzyskać odpowiedź podobną do następującej: `pip 22.3 from C:\Users\<nazwa użytkownika>\AppData\Local\Programs\Python\Python311\Lib\site-packages\pip (python 3.11)`. Należy zwrócić uwagę na wersję Pythona w nawiasie na końcu - powinna być to wersja 3.11. Jeżeli komunikat jest odmienny tj. wersja Pythona się nie zgadza, albo uzyskujemy jakąś błędną odpowiedź kontynuujemy realizację tej instrukcji - w przeciwnym wypadku przechodzimy do instalacji poetry.
2. Ponownie wchodzimy do edytora zmiennych środowiskowych (w konsoli cmd wpisujemy `rundll32.exe sysdm.cpl,EditEnvironmentVariables`) i w górnym okienku edytujemy zmienną `Path`.
3. Upewniamy się, że bezpośrednio przed ścieżką do Pythona ustawioną w poprzedniej instrukcji znajduje się dokładnie ta sama ścieżka z dodanym podkatalogiem `\Scripts` (cała ścieżka powinna być podobna do: `C:\Users\<nazwa użytkownika>\AppData\Local\Programs\Python\Python311\Scripts`.
4. Powtarzamy punkty 2. i 3. dla dolnego okienka.
5. Po zamknięciu edytora zmiennych środowiskowych restartujemy konsolę cmd i jeszcze raz wpisujemy polecenie `pip --version`. Jeżeli wszystko wykonaliśmy poprawnie, powinniśmy uzyskamy komunikat: `pip 22.3 from C:\Users\<nazwa użytkownika>\AppData\Local\Programs\Python\Python311\Lib\site-packages\pip (python 3.11)` lub podobny.
## Instalacja poetry
1. Wchodzimy do konsoli cmd (skrót `WIN+R` i wpisujemy `cmd.exe` - aby uruchomić w trybie administratora naciskamy `CTRL+SHIFT+ENTER`) i wpisujemy: `pip install pipx`.
2. Po zakończonej instalacji wpisujemy: `pipx ensurepath`.
3. Następnie upewniamy się w edytorze zmiennych środowiskowych (w konsoli cmd wpisujemy `rundll32.exe sysdm.cpl,EditEnvironmentVariables`) i edytujemy zmienną `Path` w górnym okienku.
4. Upewniamy się, że na trzeciej pozycji od góry znajduje się wpis podobny do `C:\Users\<nazwa użytkownika>\.local\bin` - może on być dodany na dole listy ścieżek, mogą być w nim niezachowane wielkie litery - w razie wątpliwości porównujemy ze ścieżką do instalacji Pythona.
5. Punkty 3. i 4. powtarzamy dla dolnego okienka.
6.  Po zamknięciu edytora zmiennych środowiskowych restartujemy konsolę cmd i wpisujemy `pipx install poetry`.
7. Po udanej instalacji powinniśmy uzyskać w odpowiedzi na polecenie: `poetry --version` komunikat podobny do następującego: `Poetry (version 1.4.1)` - oznacza to, że poprawnie zakończyliśmy konfigurację środowiska.
