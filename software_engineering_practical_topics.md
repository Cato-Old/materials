# Inżynieria oprogramowania - zagadnienia praktyczne
## Testowanie
1. Testy unitowe i testy integracyjne we frameworku Flask:
	a. testy unitowe --- z mockowanymi zależnościami, bez testowania routingu;
	b. testy integracyjne --- oryginalnymi zależnościami wewnątrzaplikcyjnymi.
	Więcej o testowaniu we flasku (chociaż materiały odnoszą się głównie do testowania integracyjnego) znajdziesz w [dokumentacji](https://flask.palletsprojects.com/en/2.2.x/testing/).
2. Testy we frameworku pytest --- pisanie prostych testów i odpalanie ich w konsoli i w IDE .(PyCharm i/lub VSCode).
3. Fixtury we frameworku pytest i dependency injection.
	Więcej o tych zagadnieniach znajdziesz w dokumentacji frameworka pytest poświęconej [fixturom](https://docs.pytest.org/en/6.2.x/fixture.html#what-fixtures-are).
4. Wbudowane fixtury ułatwiające sprawdzanie co zostało wylogowane, wypisane na konsolę typu `capsys`: [dokumentacja](https://docs.pytest.org/en/6.2.x/capture.html) im poświęcona.
5. Sprawdzanie czy został wyrzucony wyjątek: menadżer kontekstu `pytest.raises()`.
6. Podstawy mockowania: biblioteka standardowa i moduł `unittest.mock`. Sprawdzanie wywołań mocka.
## Repozytoria
1. Budowanie szkieletu repozytorium --- metody złożone z sygnatury i kodu wyrzucającego wyjątek.
2. Testowanie szkieletu repozytorium --- testy dla metod wyrzucających `NotImplementedError`.
3. Budowanie zależności w endpoincie: ręczne wstrzykiwanie zależności kontrolera do jego konstruktora/inicjalizatora (funkcji magicznej `__init__()`).
4. Testowanie użycia rezpozytorium w kontrolerze --- za pomocą odpowiednich metod obiektu `Mock`.
5. Obsługa wyjątków w endpoincie bez naruszania zachowania sprawdzanego w testach integracyjnych.
