
```markdown
# Model domeny

## Encje

- konto
- rola
- blokada
- ustawienia klienta
- pokój gry
- chat
- wiadomość
- sklep
- produkt
- transakcja
- ekwipunek
- zgłoszenie
- ankieta
- sesja gry

---

## Relacje

- konto posiada rolę
- konto posiada ekwipunek
- konto posiada ustawienia klienta
- konto wykonuje transakcję
- konto wysyła wiadomość
- konto jest autorem wiadomości
- konto składa zgłoszenie
- konto uczestniczy w pokoju gry
- konto posiada blokadę
- pokój gry posiada chat
- pokój gry posiada sesję gry
- chat zawiera wiadomości
- wiadomość może być przedmiotem zgłoszenia
- sklep oferuje produkty
- transakcja dotyczy produktu
- ekwipunek zawiera produkty

---

## Uwagi

- Encja "sesja gry" reprezentuje dane o przebiegu meczu zwracane przez serwer gry
  i przechowywane przez klienta (wyniki, historia, stan pokoju).
- Encja "ustawienia klienta" przechowuje preferencje gracza synchronizowane
  między urządzeniami (mapowanie klawiszy, głośność).
- Logika punktacji i mechaniki klas postaci należy do serwera gry —
  klient jedynie pobiera i prezentuje te dane.
```
