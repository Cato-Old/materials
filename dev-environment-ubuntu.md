# Tworzenie środowiska (Ubuntu)
## Instalacja Pythona
1. Wchodzimy do terminala i uaktualniamy indeksy **apt** za pomocą komendy: `sudo apt update`.
2. Następnie sprawdzamy wersję Pythona zainstalowaną w naszym systemie: `python3 --version`. W przypadku najnowszego Ubuntu będzie to najprawdopodobniej: `Python 3.10.6`.
3. Instalujemy wersję 3.11 Pythona za pomocą komendy: `sudo apt install python 3.11`. Po pomyślnie skończonej instalacji powinniśmy na polecenie `python3.11 --version` otrzymać w odpowiedzi komunikat: `Python 3.11.0rc1`.
4. W konsoli wpisujemy: `nano ~/.bashrc` (możemy użyć dowolnego innego edytora) i na końcu pliku dodajemy wpis: `alias python=python3.11`. Następnie wczytujemy do konsoli plik konfiguracyjny: `source ~/.bashrc` i sprawdzamy polecenie `python --version`. Jeśli wszystko wykonaliśmy poprawnie otrzymamy w odpowiedzi: `Python 3.11.0rc1`.
## Instalacja pip
1. Najprawdopodobniej w systemie nie jest zainstalowany pip dla żadnej wersji Pythona. Potrzebujemy zainstalować menedżera pakietów dla wersji 3.11. W konsoli wpisujemy: `curl -sS https://bootstrap.pypa.io/get-pip.py | python3.11`.
2. Następnie w konsoli wpisujemy: `pip3.11 --version`. Najprawdopodobniej dostaniemy komunikat, że system nie jest w stanie znaleźć takiego pliku na ścieżce. Jeżeli jednak dostaniemy odpowiedź: `pip 23.0.1 from /home/<nazwa użytkownika>/.local/lib/python3.11/site-packages/pip (python 3.11)` przechodzimy do punktu 4.
3. W konsoli wpisujemy: `nano ~/.bashrc` (możemy użyć dowolnego innego edytora). Następnie na końcu pliku dodajemy wpis: `export PATH=/home/<nazwa użytkownika>/.local/bin:$PATH`. Następnie wczytujemy plik konfiguracyjny do konsoli: `source ~/.bashrc` i sprawdzamy polecenie `pip3.11 --version`. Jeżeli wszystko ustawiliśmy poprawnie powinniśmy otrzymać odpowiedź podobną do następującej: `pip 23.0.1 from /home/<nazwa użytkownika>/.local/lib/python3.11/site-packages/pip (python 3.11)`.
4. W konsoli wpisujemy `nano ~/.bashrc` (możemy użyć dowolnego innego edytora) i dodajemy wpis: `alias pip=pip3.11`. Następnie wczytujemy plik konfiguracji do konsoli poleceniem: `source ~/.bashrc` i sprawdzamy wersję pip: `pip --version`. Powinniśmy otrzymać taką samą odpowiedź jak w przypadku polecenia `pip3.11 --version`.
## Instalacja poetry
1. W konsoli wpisujemy: `pip install pipx`. Po udanej instalacji polecenie `pipx --version` powinno zwrócić odpowiedź analogiczną do następującej: `1.2.0`.
2. Najprawdopodobniej nie mamy zainstalowanego rozszerzenia Python dla wirtualnych środowisk. Dlatego wpisujemy do konsoli: `sudo apt install python3.11-venv` i instalujemy ten pakiet.
3. W konsoli wpisujemy: `pipx install poetry`. Po zakończonym sukcesem zainstalowaniu wpisujemy do konsoli polecenie: `poetry --version` i powinniśmy ujrzeć następującą odpowiedź: `Poetry (version 1.4.1)`- oznacza to, że poprawnie zakończyliśmy instalację środowiska.
