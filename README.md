# Generator stopki e-mail

Jednoplikowy generator stopki (podpisu) e-mail. Działa w przeglądarce, bez instalacji i bez serwera.

![Przykładowa stopka](example.png)

## Użycie

1. Otwórz `index.html` w przeglądarce (lub wersję z GitHub Pages, jeśli jest włączona).
2. Wypełnij formularz. Podgląd aktualizuje się na bieżąco, dane zapisują się lokalnie w przeglądarce.
3. Kliknij **Kopiuj stopkę** i wklej ją w ustawieniach podpisu:
   - **Gmail:** Ustawienia → Zobacz wszystkie ustawienia → Ogólne → Podpis.
   - **Outlook (web / nowy Outlook):** Ustawienia → Konto → Podpisy.
   - **Thunderbird i inne:** użyj **Pobierz plik .html** i wskaż plik jako podpis HTML.

## Zgodność z klientami poczty

- Układ oparty na tabelach i stylach inline (klienci poczty usuwają `<style>` i `<head>`).
- Brak SVG (Gmail i Outlook go nie wyświetlają). Logo podaje się jako publiczny URL do PNG/JPG, bez logo generowany jest przycisk z tabeli.
- Wartości z formularza są escapowane, adresy bez protokołu dostają `https://`.

## GitHub Pages (opcjonalnie)

Settings → Pages → Source: *Deploy from a branch* → `main` / `root`. Generator będzie dostępny pod `https://<użytkownik>.github.io/e-mail-footer-generator/`.
