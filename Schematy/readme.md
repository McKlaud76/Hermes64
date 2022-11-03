Folder ze schematami przerysowanymi ze zdjęć i notatek bez zmian w konkstrukcji poszczególnych modułów. 

W przypadku jakichkolwiek wątpliwości i nieścisłości, za punkt odniesienia należy przyjąć oryginalne schematy dostępne na stronie: [http://share.leonek.org/e/hermes64/](http://share.leonek.org/e/hermes64/)

Opisy poszczególnych elekementów składowych zostały zaczerpnięte z strony powyżej:

-hermes_0001.jpeg - Clock & Counters (CC)
>Płytka CC zawierała generator zegarowy i zestaw liczników wraz z odrobiną logiki, który pozwalał wytwarzać sygnał TV i generować adresy komórek pamięci obrazu. Tutaj jest określane położenie "papera" na obrazie, dlatego multiplekser przełączający między danymi piksli obrazu (z płyty DRC) a kolorem borderu (rejestr na płycie I/O) jest właśnie tu.

>Początkowo Hermes posiadał generator zegarowy LC, który wymagał nastrojenia. Potem zastąpiłem cewkę kwarcem z Juniora.

-hermes_0002.jpeg - Display RAM Controller (DRC)

>Wykonuje najtrudniejszą funkcję, czyli rozrząd dostępu do RAM pomiędzy procesor a układ wyświetlania. Układ jest udany - zapewnia Hermesowi szybkość (odczyty RAM nie powodują wait-states, a zapisy sporadycznie) choć są tu dwa miejsca wymagające poprawki. Tu określa się organizację pamięci obrazu ZX-Spectrum.

>ZX-Spectrum zbudowany na bazie tego układu byłby szybszy, ale ULA musiałaby mieć więcej nóżek.

-hermes_0003.jpeg - CPU

-hermes_0004.jpeg - I/O

-hermes_0005.jpeg - Zasilacz
