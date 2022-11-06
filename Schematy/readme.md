Folder ze schematami przerysowanymi ze zdjęć i notatek bez zmian w konkstrukcji poszczególnych modułów. 

W przypadku jakichkolwiek wątpliwości i nieścisłości, za punkt odniesienia należy przyjąć oryginalne schematy dostępne na stronie: [http://share.leonek.org/e/hermes64/](http://share.leonek.org/e/hermes64/)

Opisy poszczególnych elekementów składowych zostały zaczerpnięte z strony powyżej:

- hermes_0001.jpeg - Clock & Counters (CC)
>Płytka CC zawierała generator zegarowy i zestaw liczników wraz z odrobiną logiki, który pozwalał wytwarzać sygnał TV i generować adresy komórek pamięci obrazu. Tutaj jest określane położenie "papera" na obrazie, dlatego multiplekser przełączający między danymi piksli obrazu (z płyty DRC) a kolorem borderu (rejestr na płycie I/O) jest właśnie tu.

>Początkowo Hermes posiadał generator zegarowy LC, który wymagał nastrojenia. Potem zastąpiłem cewkę kwarcem z Juniora.

- hermes_0002.jpeg - Display RAM Controller (DRC)

>Wykonuje najtrudniejszą funkcję, czyli rozrząd dostępu do RAM pomiędzy procesor a układ wyświetlania. Układ jest udany - zapewnia Hermesowi szybkość (odczyty RAM nie powodują wait-states, a zapisy sporadycznie) choć są tu dwa miejsca wymagające poprawki. Tu określa się organizację pamięci obrazu ZX-Spectrum.

>ZX-Spectrum zbudowany na bazie tego układu byłby szybszy, ale ULA musiałaby mieć więcej nóżek.

- hermes_0003.jpeg - CPU

>Mamy tu procesor, ROM, rejestr zgłoszenia przerwania oraz proste MMU zapewniające przełączanie banków pamięci i inne funkcje. Sygnały procesora są buforowane, bo elektronika Hermesa jest fizyczne duża i goły Z-80 mógłby nie dać rady napędzać wszystkich linii samodzielnie.

- hermes_0004.jpeg - I/O

>Płyta wejścia wyjścia. Port klawiatury, joysticka, wejście/wyjście pamięci masowej (magnetofon kasetowy). Układ RESET i NMI, dekoder adresów oraz dodatkowy port 30, specyficzny dla Hermesa, przy pomocy którego steruje się MMU, można zmienić adres pamięci obrazu a nawet całkowicie go wyłączyć. Po wyłączeniu obrazu procesor ma dostęp do pamięci bez wait-states przy wszystkich operacjach.

- hermes_0005.jpeg - Zasilacz (PSU)

>Główny zasilacz z impulsową stabilizacją oraz dwa zasilacze pomocnicze. Jest też tu zabezpieczenie, tzw. crow bar w postaci tyrystora, który ma za zadanie zewrzeć zasilacz i przepalić bezpiecznik, gdyby zasilacz się uszkodził i dawał napięcie mogące uszkodzić logikę komputera.
