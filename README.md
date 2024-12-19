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

![training_history_iris](https://github.com/user-attachments/assets/4d22759f-117d-4c1e-8925-a828072db824)


## CIFAR-10 Classification (Modified to Dense Layers Only)

Ten notebook wykorzystuje zbiór CIFAR-10 (wbudowany w Keras).
Używa wyłącznie warstw Dense.
Obrazy zostaną spłaszczone i podane do MLP.

Wyniki i wykresy zapisywane są w katalogu `logs/`.

![training_history_cifar10](https://github.com/user-attachments/assets/0481adb2-e628-4933-9a28-da525a90b78c)


## Fashion-MNIST Classification (Modified to Dense Layers Only)

Ten notebook wykorzystuje zbiór Fashion-MNIST (wbudowany w Keras) i trenuje model MLP.

Rysujemy również macierz pomyłek, a wyniki i logi zapisujemy w katalogu `logs/`.

![training_history_fashion_mnist](https://github.com/user-attachments/assets/fef88f94-907b-4c09-8795-23f5e64d4ff0)
![confusion_matrix](https://github.com/user-attachments/assets/c7b88078-284f-47c5-8710-a505bb6c9bee)


## Wine Classification

Ten notebook korzysta z zbioru Wine (z sklearn), klasyfikując rodzaje wina (3 klasy)
na podstawie cech chemicznych. Porównuje dwa modele o różnej wielkości:
1. Mały model (jedna ukryta warstwa)
2. Większy, głębszy model

Wyniki są zapisywane w katalogu `logs/`.


![training_history_wine_small](https://github.com/user-attachments/assets/f92b2623-7b09-4885-87d8-646785b19098)
![training_history_wine_large](https://github.com/user-attachments/assets/bc60c05e-2c52-4b9b-866f-90984a0d19c6)

