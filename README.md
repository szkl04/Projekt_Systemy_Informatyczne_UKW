# System klienta gry wieloosobowej

Projekt wykonany w ramach przedmiotu **Systemy Informatyczne** na Uniwersytecie Kazimierza Wielkiego w Bydgoszczy.

## Opis projektu

Projekt przedstawia koncepcję systemu klienckiego dla gry wieloosobowej. Nie obejmuje implementacji samej mechaniki gry, ta należy do przyszłego serwera gry, lecz opisuje warstwę kliencką odpowiedzialną za zarządzanie kontami, komunikację, sklep, moderację i interfejs użytkownika.

System obsługuje cztery role użytkowników: **gracza**, **moderatora**, **Product Managera** oraz **administratora**.

## Zakres funkcjonalny

### Gracz
- Rejestracja i logowanie, zarządzanie profilem (awatar, nazwa konta)
- Tworzenie i dołączanie do pokoi gry (bezpośrednio lub przez kod zaproszenia)
- Wybór klasy postaci i zakup skórek w wewnętrznym sklepie
- Czat tekstowy (drużynowy i prywatny) z obsługą skrótów klawiszowych
- Przeglądanie rankingu, historii rozgrywek i statystyk
- Personalizacja ustawień klawiszy i dźwięku synchronizowana między urządzeniami
- Zgłaszanie nieodpowiednich zachowań innych graczy
- Codzienna nagroda za logowanie i ankiety po meczu

### Moderator
- Panel zarządzania: lista zgłoszeń, aktywne pokoje, podgląd czatu
- Nakładanie blokad na konta (czasowych lub stałych) i wyciszanie graczy na czacie
- Zamykanie pokoi, resetowanie rundy i wymuszanie zakończenia meczu

### Product Manager
- Raporty sprzedaży sklepu z filtrami dat i rozróżnieniem przychodów z promocji
- Statystyki aktywności graczy w czasie rzeczywistym (DAU, wykres 24h)
- Konfiguracja nagród dziennych i zarządzanie ankietami po meczu

### Administrator
- Nadawanie i odbieranie ról użytkownikom (moderator, Product Manager) ze skutkiem natychmiastowym
- Historia zmian ról

## Model domeny

Projekt obejmuje następujące encje: **konto**, **rola**, **blokada**, **ustawienia klienta**, **pokój gry**, **sesja gry**, **chat**, **wiadomość**, **sklep**, **produkt**, **transakcja**, **ekwipunek**, **zgłoszenie**, **ankieta**.

Logika punktacji i mechaniki klas postaci należy do serwera gry - klient jedynie pobiera i prezentuje te dane. Ustawienia gracza są synchronizowane między urządzeniami.

## Artefakty projektowe

- Model domeny
- Diagram ERD
- User Stories z kryteriami akceptacji (24 historyjki)
- Diagramy User Flow:
  - Zakup przedmiotu w sklepie
  - Wysłanie wiadomości prywatnej
- Makiety UI odpowiadające powyższym przepływom

---

*Projekt studencki autorstwa Szymona Laskowskiego i Jana Nowaka - Systemy Informatyczne, UKW*
