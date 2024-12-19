### NAI 05

Autorzy:
- Kacper Sewruk s23466
- Michał Jastrzemski s26245

## Opis
Cztery zadania związane z klasyfikacją w TensorFlow/Keras.  
1. **Iris**: Klasyfikacja gatunków kwiatów. Porównanie MLP z modelem jednopoziomowym.  
2. **CIFAR-10**: Klasyfikacja obrazów za pomocą warstw Dense (obrazy spłaszczone).  
3. **Fashion-MNIST**: Klasyfikacja ubrań, trening MLP, macierz pomyłek.  
4. **Wine**: Klasyfikacja gatunków wina, porównanie małej i dużej sieci.


## Iris Classification - Neural Network vs. Simple Model

Ten notebook wczytuje zbiór danych Iris z pliku iris.csv, dokonuje podziału
na zbiory treningowy i testowy, normalizuje dane, a następnie trenuje dwie sieci neuronowe:
1. MLP (wielowarstwowy perceptron) do klasyfikacji gatunków Iris.
2. Model z pojedynczą warstwą Dense (odpowiednik regresji logistycznej), również w Keras.

Na koniec wyniki obu modeli są porównywane, a logi i wykresy zapisywane w katalogu `logs/`.

## CIFAR-10 Classification (Modified to Dense Layers Only)

Ten notebook wykorzystuje zbiór CIFAR-10 (wbudowany w Keras).
Używa wyłącznie warstw Dense.
Obrazy zostaną spłaszczone i podane do MLP.

Wyniki i wykresy zapisywane są w katalogu `logs/`.

## Fashion-MNIST Classification (Modified to Dense Layers Only)

Ten notebook wykorzystuje zbiór Fashion-MNIST (wbudowany w Keras) i trenuje model MLP.

Rysujemy również macierz pomyłek, a wyniki i logi zapisujemy w katalogu `logs/`.

## Wine Classification

Ten notebook korzysta z zbioru Wine (z sklearn), klasyfikując rodzaje wina (3 klasy)
na podstawie cech chemicznych. Porównuje dwa modele o różnej wielkości:
1. Mały model (jedna ukryta warstwa)
2. Większy, głębszy model

Wyniki są zapisywane w katalogu `logs/`.
