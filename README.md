# Analiza danych pingwinów i budowa modeli regresji

## Opis projektu

Projekt polega na analizie danych dotyczących pingwinów oraz budowie modeli regresji w celu wyjaśnienia zmienności masy ciała pingwinów na podstawie różnych cech, takich jak długość dzioba, szerokość dzioba i długość płetwy. W ramach projektu zostały wykorzystane dwa podejścia:

1. **Regresja liniowa** – prosty model wykorzystujący liniową zależność między zmiennymi.
2. **Regresja wielomianowa** – bardziej złożony model pozwalający uchwycić nieliniowe zależności między zmiennymi.

## Dane wejściowe

Plik CSV `pingwiny 2.csv` zawiera dane o pingwinach, w tym następujące kolumny:
- `gatunek` – gatunek pingwina,
- `wyspa` – wyspa, na której żyje pingwin,
- `dlugosc_dzioba_mm` – długość dzioba (w mm),
- `szerokosc_dzioba_mm` – szerokość dzioba (w mm),
- `dlugosc_pletwy_mm` – długość płetwy (w mm),
- `masa_ciala_g` – masa ciała pingwina (w gramach),
- `plec` – płeć pingwina.

## Cele projektu

1. Prawidłowe wczytanie danych i przygotowanie ich do analizy.
2. Zbudowanie modelu regresji liniowej, którego równanie opisuje zależność między masą ciała a pozostałymi zmiennymi.
3. Zinterpretowanie istotności zmiennych, współczynnika determinacji \( R^2 \) oraz wartości p modelu.
4. Zweryfikowanie jakości modelu poprzez analizę reszt i predykcję masy ciała dla konkretnych przypadków.
5. Stworzenie konkurencyjnego modelu (np. regresji wielomianowej) z \( R^2 \geq 0.75 \).
6. Porównanie wyników obu modeli i wskazanie lepszego podejścia.

## Wykorzystane technologie

- Python
- Biblioteki: `pandas`, `numpy`, `matplotlib`, `seaborn`, `statsmodels`, `sklearn`

## Struktura projektu

- `pingwiny 2.csv` – dane wejściowe do analizy.
- `pingwiny.ipynb` – główny skrypt przeprowadzający analizę i budowę modeli regresji.
- `README.md` – opis projektu.

## Wyniki

1. Model regresji liniowej osiągnął \( R^2 \approx 0.54 \), co oznacza umiarkowane wyjaśnienie zmienności masy ciała pingwina.
2. Model regresji wielomianowej (stopień 2) osiągnął \( R^2 \geq 0.75 \), co oznacza lepsze dopasowanie do danych.
3. Regresja wielomianowa lepiej sprawdza się w predykcji, gdy zależność między zmiennymi jest nieliniowa, jednak jest bardziej złożona.
