# covid19-vaccination-analysis
## Opis projektu
Projekt analityczny w Pythonie badający postępy szczepień przeciw COVID-19 w UE. Wykorzystuje biblioteki Pandas i Seaborn do analizy czasowej, agregacji, porównań między państwami oraz analizy demograficznej grup wiekowych w Polsce.

## Zbiór danych
Analiza opiera się na pliku z danymi (w kodzie wczytywanym jako `data.csv`), który zawiera oficjalne raporty dotyczące liczby szczepień w krajach UE. Dane obejmują m.in.:
* Liczbę podanych pierwszych i drugich dawek w ujęciu tygodniowym (`YearWeekISO`).
* Podział na kraje (`ReportingCountry`) i regiony.
* Grupy docelowe (np. `ALL` - cała populacja, `HCW` - pracownicy ochrony zdrowia, oraz poszczególne grupy wiekowe, np. `Age18_24`, `Age80+`).
* Rodzaje podanych szczepionek (np. COM, MOD, AZ).

## Główne zadania i analizy wizualne
Projekt został podzielony na trzy główne etapy analityczne:
1. **Analiza miesięczna**: Agregacja i wizualizacja łącznej liczby osób zaszczepionych pierwszą dawką w poszczególnych krajach w każdym miesiącu 2021 roku. Wykresy słupkowe zostały posortowane rosnąco, co ułatwia analizę porównawczą.
2. **Porównanie krajów**: Obliczenie i zaprezentowanie narastającej liczby osób w pełni zaszczepionych w ujęciu tygodniowym dla czterech kluczowych państw: **Polski, Hiszpanii, Francji i Włoch**.
3. **Analiza demograficzna w Polsce**: Analiza przebiegu szczepień pierwszą dawką w czasie z podziałem na 6 kluczowych grup wiekowych w Polsce (od 18 lat do 80+), obrazująca priorytetyzację grup najstarszych w pierwszych fazach programu.

## Technologie i Biblioteki
Projekt opiera się na stosie technologicznym Pythona przeznaczonym do analizy i wizualizacji danych:
* `pandas` i `numpy` – do manipulacji danymi, grupowania, tworzenia tabel przestawnych oraz obliczania sum skumulowanych.
* `matplotlib.pyplot` i `seaborn` – do tworzenia estetycznych i czytelnych wykresów z odpowiednimi etykietami i legendami.

## Jak uruchomić projekt
1. Sklonuj repozytorium na swój dysk.
2. Upewnij się, że masz zainstalowane środowisko Python z pakietami wymienionymi wyżej.
3. Projekt był tworzony z myślą o środowisku Google Colab. Jeśli chcesz go tam uruchomić, wywołaj pierwszą komórkę z google.colab.files.upload() i wgraj plik .csv.
4. Aby uruchomić go lokalnie, wystarczy umieścić plik `data.csv` w jednym folderze z notatnikiem i pominąć komórkę odpowiedzialną za upload.
5. Uruchamiaj kolejne komórki kodu.
