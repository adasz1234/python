# PC Creator
## 1. Opis
PC Creator pozwala w łatwy sposób na skomplementowanie listy wymaganych podzespołów do złożenia w pełni funkcjonalnego komputera stacjonarnego. Dla zaawansowanych użytkowników ma to być miejsce na szybkie wyszukanie lub stworzenie listy odpowiednich komponentów. Jednakże dla niej zaawansowanych lub dopiero zaczynających swoją przygodę z komputera ma na celu umożliwić łatwiejszy wybór między komputerem „gotowcem” a  samodzielnym skomplementowaniu i złożeniu własnego komputera, który  może  być w przyszłości rozbudowany. Dzięki opcjonalnej możliwości filtrowania według kompatybilności użytkownicy nie muszą się martwić przypadkowym zakupem podzespołów które finalnie nie będą ze sobą  współpracowały. Użytkownicy mogą także opcjonalnie
założyć konto aby zapisać stworzoną listę na później.


## 2. Wymagania funkcjonalne:
- [ ] Przejrzysty widok komponentów,
- [ ] Możliwość tworzenia kompletnej listy podzespołów,
- [ ] Automatyczne ukrywanie niekmpatybilnych komponentów,
- [ ] Możliwość filtrowania podzespołów,
- [ ] Opcja widoku uproszczonego dla mniej zaawansowanych,

## 3. UX
### Strona główna
<img alt="Strona główna"
     src="https://github.com/pwr-wefim-po-2026/programowanie-obiektowe-287277/blob/main/287277/strona_glowna.jpg"
     width="450">
### Wybór
 <img alt="Wybór"
     src="https://github.com/pwr-wefim-po-2026/programowanie-obiektowe-287277/blob/main/287277/wybor.jpg"
     width="450">
### Lista
<img alt="Lista"
     src="https://github.com/pwr-wefim-po-2026/programowanie-obiektowe-287277/blob/main/287277/lista.jpg"
     width="450">
### Rejestracja i logowanie
 <img alt="Rejestracja i logowanie"
     src="https://github.com/pwr-wefim-po-2026/programowanie-obiektowe-287277/blob/main/287277/login.jpg"
     width="450">

## 4. Modele:

### Uzytkownik
| Atrybut  | Typ     | Opis                         |
|----------|---------|------------------------------|
| id_user  | int     | Klucz główny użytkownika     |
| email    | varchar | Adres e-mail użytkownika     |
| haslo    | varchar | Zaszyfrowane hasło           |
| imie     | varchar | Imię użytkownika             |

### Procesor
|     Atrubut    | Typ  |                  Opis                   |
|----------------|------|-----------------------------------------|
|  id_gniazdo    | char | Typ gniazda                             |
| id_producent_p | char | Nazwa producenta                        |
|  id_rdzenie    | int  | Ilość rdzenii                           |
| id_generacja   | int  | Generacja procesora                     |
| id_model       | int  | Model procesora                         |
| id_integra     | int  | Obecność zintegrowanej karty graficznej |

### Pamięć RAM
|    Atrybut    | Typ  |                 Opis                  |
|---------------|------|---------------------------------------|
|    id_slot    | char | Typ gniazda pamięci                   |
| id_taktowanie | int  | Prędkość tatkowania                   |
| id_pojemnosc  | int  | Pojemność pojemność pojedyńczej kości |
| id_cl_rating  | int  | Opóźnienie pamięci                    |

### Płyta główna
|   Atrybut   | Typ  |                 Opis                |
|-------------|------|-------------------------------------|
| id_SLOT     | char | Rodzaj kompatybilnej paięci RAM     |
| id_GNIAZDO  | char | Rodzaj gniazda procesora            |
| id_wifi     | char | Obecność i typ karty sieciowej wifi |
| id_ethernet | int  | Maksymalna przepustowość ethernet   |
| id_SATA     | int  | Ilość złączy typu SATA              |
| id_NVME     | int  | Ilość slotów na dyski M.2           |
| id_typ      | char | Rozmiar płyty głównej               |
| id_chipset  | char | Chipset płyty głównej               |

### Karta graficzna
|       Atrybut        | Typ  |        Opis            |
|----------------------|------|------------------------|
| id_manufacturer      | char | Producent              |
| id_vram              | int  | Ilość pamięci VRAM     |
| id_generaction_model | char | Model karty graficznej |
| id_generaction       | int  | Generacja              |

### Dysk
|    Atrybut   | Typ  |        Opis            |
|--------------|------|------------------------|
| id_pojemnosc | char | Pojemność              |
| id_rodzaj    | int  | Rodzaj dysku           |
| id_zapis     | char | Prędkość zapisu        |
| id_odczyt    | int  | Prędkość odczytu       |
| id_rozmiar   | int  | Rozmiar fizyczny dysku |

### Zasilacz
|    Atrybut    | Typ  |         Opis           |
|---------------|------|------------------------|
| id_moc        | int  | Moc maksymalna         |
| id_certyfikat | char | Rodzaj certyfikatu 80+ |
