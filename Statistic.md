# Ta sekcja zawiera moje notatki z lektury "Statystyka praktyczna w Data Science".

## Badania eksploracyjne

### Kluczowe pojęcia dotyczące typów danych
* **Numeryczne**: Dane wyrażane w skali numerycznej
   * `Ciągłe`: Dane, które mogą przyjmować dowolną wartość z przedziału (Synonimy: przedziałowe, numeryczne, float)
   * `Dyskretne`: Dane, które mogą przyjmować jedynie wartości całkowite, np. liczność (Synonimy: zliczenia, integer)
* **Skategoryzowane**: Dane, które mogą przyjmować jedynie wartości z konkretnego zbioru, reprezentującego możliwe kategorie
  * `Binarne`: Szczególny przypadek danych skategoryzowanych z dwoma wartościami np. 0/1, true/false
  * `Porządkowe`: Dane skategoryzowane według wprowadzonego porzadku.

**Określenie typu danych w oprogramowaniu jest sygnałem dla niego, w jaki sposób dane mają być przetwarzane.**

### Kluczowe pojęcia dotyczące danych stabelaryzowanych
* `Ramka danych`: Dane stabelaryzowane (jak arkusz kalkulacyjny) są podstawową strukturą w statystyce i modelach uczenia maszynowego.
* `Cecha`: Kolumna w tabeli jest najczęściej nazywana cechą (Synonimy: atrybut, wejście, predyktor, zmienna).
* `Wynik`: Wiele projektów w data science służy do przewidywania wyniku - zazwyczaj w postaci tak/nie. Cechy są czasem wykorzystywane do przewidzenia wyniku w badaniach eksperymentalnych (Synonimy: zmienna zależna, odpowiedź, cel, wyjście).
* `Rekord`: Wiersz w tabeli jest najczęściej nazywany rekordem (Synonimy: przypadek, przykład, instancja, obserwacja, wzorzec, próbka).
