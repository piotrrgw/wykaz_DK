# Kalkulator Minut Niebezpiecznych (Hazardous Duty Time Calculator)

Aplikacja webowa wspierająca pracę drużyn konduktorskich, służąca do automatycznego obliczania sumy tzw. "minut niebezpiecznych" na podstawie wykazu pracy. Narzędzie eliminuje konieczność ręcznego sumowania czasów z poszczególnych czynności, zapewniając precyzję rozliczeń zgodnie z przyjętymi normatywami.

## 🚀 Kluczowe Funkcjonalności

System analizuje harmonogram służby i automatycznie wyodrębnia czas pracy w warunkach szczególnych/niebezpiecznych według zaimplementowanego algorytmu:

* **Obsługa wykazu pracy:** Możliwość wprowadzenia danych dotyczących czynności służbowych (godziny rozpoczęcia i zakończenia).
* **Ciągłość czasu pracy (Midnight Crossing):** Aplikacja posiada wbudowaną logikę obsługi **przełomu dób**. Poprawnie kalkuluje czas trwania czynności, które rozpoczynają się w jednym dniu kalendarzowym, a kończą w następnym.
* **Automatyczna sumaryzacja:** Generowanie łącznego raportu minut podlegających pod dodatek/rozliczenie.

## ⚙️ Algorytm Naliczania

Aplikacja opiera obliczenia na sztywno zdefiniowanych regułach (parametryzacja czynności):

| Czynność Służbowa | Wartość naliczana (Minuty Niebezpieczne) |
| :--- | :--- |
| **Przyjęcie pociągu** | Stała wartość: **20 minut** |
| **Zdanie pociągu** | Stała wartość: **10 minut** |
| **Wykonywanie próby hamulca** | **Pełny wymiar czasu** trwania czynności (zgodnie z czasem rzeczywistym) |

## 🤖 AI-Assisted Development

Projekt został zrealizowany w modelu **AI-Assisted Development** przy wsparciu modelu językowego **ChatGPT**. Sztuczna inteligencja została wykorzystana do:

* Opracowania logiki obliczania różnic czasowych (Time Delta) z uwzględnieniem zmiany daty.
* Zaimplementowania warunków logicznych przypisujących odpowiednie wagi czasowe do konkretnych czynności służbowych.
* Optymalizacji kodu pod kątem wydajności i czytelności.

## 🛠️ Stack Technologiczny

* HTML5
* CSS3
* JavaScript (ES6+)
