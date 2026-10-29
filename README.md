# Cześć, jestem Adrian 👋

Przez prawie 8 lat prowadziłem firmę transportową (podwykonawca DHL). Teraz łączę znajomość logistyki i małego biznesu z technologią.
Buduję działające narzędzia dla prawdziwych użytkowników: od aplikacji iOS dla kierowców po system rezerwacji, na którym działa prawdziwy salon.
Pracuję z asystentami AI do programowania (Claude Code), a sam odpowiadam za pomysł, wymagania, testy, wdrożenie i utrzymanie.

📍 Warszawa i okolice · 💼 [LinkedIn](https://www.linkedin.com/in/adrian-janicki-587b79447) · ✉️ adrian.janicki0@gmail.com

---

## 💅 System rezerwacji online dla salonu beauty
**Działa produkcyjnie:** [paznokciekaliszki.pl](https://paznokciekaliszki.pl) – Julia Królak Beauty Studio

<p>
  <img src="images/booking-desktop.png" alt="Strona salonu – komputer" width="68%">
  <img src="images/booking-mobile.png" alt="Strona salonu – telefon" width="24%">
</p>

- Rezerwacja wizyt online z dostępnymi terminami pobieranymi na żywo z **Google Calendar** (OAuth 2.0).
- Klientka sama zmienia lub odwołuje wizytę w panelu „Moja rezerwacja”.
- Automatyczne e-maile: potwierdzenia, podziękowania po wizycie i przypomnienia o kolejnej (zadania **cron**, Resend).
- Jedno źródło prawdy o godzinach otwarcia i cenniku, wspólne dla frontendu i backendu, z testem, który blokuje wdrożenie, gdy dane się rozjadą.
- **CI/CD w GitHub Actions:** każdy push uruchamia testy wyglądu w przeglądarce (telefon, tablet, komputer), a po ich przejściu strona wdraża się sama. Pliki podmieniane są atomowo, więc strona nigdy nie jest „w połowie wgrana”.
- SEO: dane strukturalne schema.org, sitemap, polityka prywatności i zgody na cookies.

`Node.js` `Express` `Google Calendar API` `HTML/CSS/JavaScript` `GitHub Actions` `cron`
*(kod prywatny – zawiera dane klientów)*

---

## 🚚 WaybillRouter – aplikacja iOS dla kierowcy
**Kod:** [github.com/adrianjanicki/Waybill-Router](https://github.com/adrianjanicki/Waybill-Router)

Problem z mojej pracy: ręczne przepisywanie listów przewozowych i liczenie kilometrów do kart drogowych.
- Skanowanie listu przewozowego aparatem i **OCR** (Apple Vision) – aplikacja sama wyciąga firmy i datę.
- **TomTom API** układa optymalną kolejność przystanków (Magazyn → firmy → Magazyn) dla profilu ciężarówki i liczy kilometry.
- Historia kursów, miesięczne podsumowanie oraz **eksport kart drogowych do PDF i zestawienia CSV do Excela**.
- Automatyczne buildy i wydania przez GitHub Actions.

`Swift` `SwiftUI` `SwiftData` `Vision/OCR` `TomTom API` `GitHub Actions`

---

## 📊 Analiza statystyk meczowych (dane + PostgreSQL)
Pipeline danych, który co tydzień pobiera wyniki i statystyki meczów z kilku zewnętrznych API, zapisuje je w bazie i liczy agregaty.
- Import danych z wielu źródeł z obsługą stronicowania i **dziennych limitów zapytań** (licznik w bazie).
- Model danych w **PostgreSQL**: mecze, statystyki drużyn i sędziów, agregaty dla ligi, sezonu i ostatnich 5/10 meczów.
- Funkcja scoringowa i ranking meczów, testy automatyczne (`node --test`), harmonogram cron.

`Node.js` `PostgreSQL` `REST API` `ETL` `cron`
*(kod prywatny)*

---

## 🏠 Homelab i automatyzacje
- Własny serwer: **Proxmox**, kontenery **Docker**, **Home Assistant**, Linux.
- Automatyczne kopie zapasowe i zadania cron, w tym codzienny backup kalendarza rezerwacji.
- Automatyczny digest treści z Reddita z wykorzystaniem agentów AI.

---

### Czego szukam
Pracy przy komputerze, zdalnej lub hybrydowej, w której przyda się połączenie logistyki od środka z technologią: planowanie transportu, koordynacja floty, wsparcie IT, automatyzacja procesów lub analiza operacyjna.
