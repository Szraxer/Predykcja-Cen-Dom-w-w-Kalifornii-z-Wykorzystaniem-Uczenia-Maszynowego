# Predykcja Cen Domów w Kalifornii z Wykorzystaniem Uczenia Maszynowego

## Cel Projektu
Celem projektu jest zbudowanie i ocena modeli regresji w celu przewidywania mediany wartości domów w dzielnicach Kalifornii. Projekt obejmuje standardowy proces uczenia maszynowego, począwszy od analizy i wstępnego przetwarzania danych, poprzez implementację różnych algorytmów regresji, aż po ocenę ich wydajności.

## Źródło Danych
Dane wykorzystane w projekcie pochodzą z platformy Kaggle i są powszechnie używane do zadań regresji.

* **Link do źródła**: [https://www.kaggle.com/datasets/camnugent/california-housing-prices](https://www.kaggle.com/datasets/camnugent/california-housing-prices)

Zbiór danych zawiera następujące atrybuty (zmienne objaśniające), opisujące każdą dzielnicę:
1.  **longitude**: długość geograficzna
2.  **latitude**: szerokość geograficzna
3.  **housing_median_age**: mediana wieku budynków w dzielnicy
4.  **total_rooms**: całkowita liczba pokoi
5.  **total_bedrooms**: całkowita liczba sypialni
6.  **population**: liczba mieszkańców
7.  **households**: liczba gospodarstw domowych
8.  **median_income**: mediana dochodów gospodarstw domowych
9.  **median_house_value** (zmienna docelowa): mediana wartości domu w dzielnicy

## Dotychczasowe Kroki Realizacji Projektu
### 1. Analiza i Wstępne Przetwarzanie Danych
W tej fazie wykonano następujące kroki:
* **Wczytanie danych**: Zbiór danych został wczytany przy użyciu biblioteki `pandas`.
* **Eksploracja danych (EDA)**: Przeprowadzono podstawową analizę statystyczną i wizualną danych w celu zrozumienia ich rozkładu i wzajemnych zależności.
* **Obsługa brakujących wartości**: Wyszukano i obsłużono brakujące dane, np. w kolumnie `total_bedrooms`.
* **Inżynieria cech**: Prawdopodobnie utworzono nowe cechy, takie jak stosunek liczby pokoi do gospodarstw domowych, aby poprawić wydajność modelu.
* **Podział danych**: Dane zostały podzielone na zbiory treningowy i testowy, aby ocenić wydajność modeli na niewidzianych wcześniej danych.

### 2. Implementacja i Ocena Modeli Regresji
Zaimplementowano i wstępnie oceniono różne modele, aby znaleźć najlepsze podejście do predykcji cen. Typowe modele w tego typu projekcie to:
* **Regresja Liniowa**: Prosty model bazowy, służący jako punkt odniesienia.
* **Drzewa Decyzyjne**: Model nieliniowy, który może lepiej uchwycić złożone zależności w danych.
* **Random Forest**: Zbiór drzew decyzyjnych, który zwykle zapewnia lepszą dokładność i jest mniej podatny na przeuczenie.

### 3. Zestawienie Porównawcze Wyników
Po wytrenowaniu i ocenie modeli, ich wydajność została porównana za pomocą metryk regresji. Tabela lub wykres porównawczy pozwolił na wizualne zestawienie wyników, co ułatwia wybór najlepszego modelu. Typowe metryki do oceny modeli regresji obejmują:
* **Mean Squared Error (MSE)**
* **Root Mean Squared Error (RMSE)**
* **R-squared ($R^2$)**
