# RMA Automotive — Analiza zgłoszeń serwisowych w Power BI

## 📊 O projekcie

Projekt przedstawia interaktywny raport analityczny przygotowany w **Microsoft Power BI**, dotyczący zgłoszeń serwisowych w branży motoryzacyjnej.

Celem projektu jest analiza liczby zgłoszeń, kosztów napraw, efektywności pracy serwisu, obsługi gwarancyjnej oraz satysfakcji klientów.

Raport składa się z czterech stron, które pozwalają analizować dane z różnych perspektyw biznesowych.

## 🛠️ Wykorzystane technologie i narzędzia

Microsoft Power BI Desktop — budowa interaktywnego raportu analitycznego

Modelowanie danych — organizacja danych w tabelach faktów i wymiarów, m.in. dotyczących dat, produktów, lokalizacji, statusów i techników

Miary analityczne w Power BI — obliczanie i prezentacja wskaźników KPI, takich jak liczba zgłoszeń, koszty napraw, średni czas naprawy i realizacja SLA

Wizualizacja danych — wykresy liniowe, kolumnowe, punktowe, macierze i drzewo dekompozycji

Analiza biznesowa — porównywanie wyników serwisu, kosztów, marek i oddziałów

## 🗂️ Model danych

Raport wykorzystuje model obejmujący tabelę faktów FACT_RMA oraz tabele wymiarów:

DIM_DATE — analiza danych w czasie

DIM_PRODUCT — marki i typy produktów

DIM_LOCATION — kraje i oddziały serwisowe

DIM_STATUS — statusy zgłoszeń

DIM_TECHNICIAN — technicy serwisowi

Taka organizacja danych umożliwia analizowanie wskaźników z różnych perspektyw biznesowych.



## 📈 Strony raportu

### 1. Executive Dashboard — przegląd wyników

Pierwsza strona przedstawia ogólny obraz działalności serwisowej.

**Zakres analizy:**
- Liczba zgłoszeń w poszczególnych latach
- Koszty napraw w podziale na marki samochodów
- Statusy zgłoszeń serwisowych
- Średni czas naprawy
- Porównanie wyników poszczególnych marek

**Podgląd dashboardu:**

<img width="1280" height="719" alt="image" src="https://github.com/user-attachments/assets/253d7c5d-5a51-4e1c-8909-1f5bcaa0f9c2" />


### 2. Service Operations — efektywność serwisu

Druga strona koncentruje się na analizie pracy techników oraz oddziałów serwisowych.

**Zakres analizy:**
- Liczba zgłoszeń obsługiwanych przez techników
- Średni czas realizacji napraw
- Średnia ocena satysfakcji klientów
- Realizacja wskaźnika SLA
- Porównanie kosztów i czasu napraw między oddziałami

**Podgląd dashboardu:**

<img width="1279" height="716" alt="image" src="https://github.com/user-attachments/assets/4c93d923-54c6-4dc2-8465-fa7f57bcf845" />


### 3. Product & Warranty — produkty i gwarancje

Trzecia strona przedstawia analizę zgłoszeń związanych z produktami oraz naprawami gwarancyjnymi.

**Zakres analizy:**
- Liczba zgłoszeń w podziale na marki
- Liczba napraw gwarancyjnych
- Koszty napraw poszczególnych typów produktów
- Średni czas naprawy
- Szczegółowe porównanie produktów i marek

**Podgląd dashboardu:**

<img width="1279" height="717" alt="image" src="https://github.com/user-attachments/assets/826f4b4a-fda9-4ce7-9ed6-ded341067989" />


### 4. Forecast & Trends — trendy i prognoza

Ostatnia strona przedstawia zmiany wybranych wskaźników w czasie.

**Zakres analizy:**
- Trend liczby zgłoszeń
- Wizualizacja prognozy liczby zgłoszeń
- Miesięczne koszty napraw
- Zmiany satysfakcji klientów
- Porównanie danych między latami

**Podgląd dashboardu:**

<img width="1279" height="720" alt="image" src="https://github.com/user-attachments/assets/6de23fa5-79e2-46e4-a598-455033b6d58a" />


## 📌 Analizowane wskaźniki KPI

| Wskaźnik | Znaczenie |
|---|---|
| Total Tickets | Łączna liczba zgłoszeń serwisowych |
| Total Cost | Łączny koszt napraw |
| Avg Repair Days | Średni czas naprawy |
| Avg Satisfaction | Średnia ocena satysfakcji klientów |
| SLA Met % | Odsetek zgłoszeń spełniających wymagania SLA |
| Warranty Repairs | Liczba napraw gwarancyjnych |

## 🔎 Przykładowe wnioski z analizy

Na podstawie danych przedstawionych w raporcie:

Audi generuje największą liczbę zgłoszeń i najwyższe łączne koszty napraw. W analizowanym zbiorze odnotowano około 1,06 mln zgłoszeń tej marki i 971 mln jednostek kosztu.

Średni czas naprawy jest zbliżony dla wszystkich analizowanych marek. Wynosi około 8,4 dnia, co wskazuje na niewielkie różnice między markami na poziomie zagregowanym.

Większość zgłoszeń ma status zamknięty. Stanowią one około 71,8% wszystkich zgłoszeń, natomiast pozostałe znajdują się na innych etapach obsługi.

Wskaźnik realizacji SLA różni się między oddziałami. Na przedstawionym wykresie wartości mieszczą się w przybliżeniu w przedziale 74–75%, co pozwala porównywać efektywność poszczególnych lokalizacji.
Przykładowe pytania, na które warto odpowiedzieć:

- Która marka generuje największe koszty napraw?
- Czy poszczególne oddziały różnią się czasem realizacji napraw?
- Jak zmienia się liczba zgłoszeń w czasie?
- Czy wyższe koszty serwisowe wiążą się z większą liczbą zgłoszeń?

## 📂 Struktura repozytorium

```text
RMA-Automotive-PowerBI/
├── README.md
├── RMA_AUTOMOTIVE.pbix
├── RMA_Automotive_Report.pdf
├── 01-executive-dashboard.png
├── 02-service-operations.png
├── 03-product-warranty.png
└── 04-trends.png
```

## 🚀 Jak uruchomić projekt?

1. Pobierz plik `RMA_AUTOMOTIVE.pbix` z repozytorium.
2. Otwórz go w **Microsoft Power BI Desktop**.
3. Przeglądaj poszczególne strony raportu.
4. Korzystaj z filtrów, aby analizować dane według marek, lat, oddziałów i innych dostępnych wymiarów.

Jeśli nie masz Power BI Desktop, możesz obejrzeć zrzuty ekranu zamieszczone powyżej lub otworzyć raport w formacie PDF.

## 👤 Autor

**Mateusz Poręba**

Projekt uczelniany — analiza danych i raportowanie biznesowe w Power BI.

