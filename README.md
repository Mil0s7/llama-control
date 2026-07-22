# Llama Control

**Llama Control** to darmowa aplikacja na komputer, która pomaga uruchamiać i ogarniać modele AI (takie jak lokalny "ChatGPT") na własnym sprzęcie — bez internetu, bez abonamentu, bez wysyłania niczego na zewnątrz.

## Jak to działa (po ludzku)

Modele AI trzymane są lokalnie na Twoim dysku jako pliki. Żeby taki model "ożył" i można było z nim rozmawiać, potrzebny jest silnik, który go uruchomi — nazywa się **llama.cpp**.

Llama Control to wygodna nakładka na ten silnik:

- **Pilnuje Twoich modeli** — pokazuje listę, ile ważą, kiedy je pobrano, pozwala je oznaczać jako ulubione i opisywać.
- **Sam zainstaluje silnik llama.cpp**, jeśli go jeszcze nie masz — dobiera odpowiednią wersję pod Twoją kartę graficzną.
- **Uruchamia i zatrzymuje model jednym kliknięciem** — bez wpisywania niczego w konsoli.
- **Pozwala pobierać nowe modele** prosto z serwisu HuggingFace (to taki "sklep" z modelami AI) i od razu mówi, czy dany model zmieści się w pamięci Twojej karty graficznej.
- **Sama się aktualizuje**, gdy pojawi się nowa wersja.

Krótko: instalujesz, apka sama dogaduje resztę, Ty tylko klikasz.

## Na jakich urządzeniach to działa

- **Tylko Windows** (10 lub 11) — komputer stacjonarny lub laptop. Nie działa na telefonach, tabletach ani na Macu/Linuksie.
- **Karta graficzna NVIDIA (GeForce/RTX) jest zalecana** — wtedy modele AI działają szybko. Bez niej też zadziała, ale wolniej (na samym procesorze).
- Modele AI potrafią ważyć od kilku do kilkudziesięciu gigabajtów, więc warto mieć trochę wolnego miejsca na dysku.

## Jak zacząć

1. Pobierz najnowszy instalator z zakładki **[Releases](../../releases)** po prawej stronie tej strony.
2. Uruchom pobrany plik `.exe`.
3. Windows może pokazać niebieski ekran ostrzegawczy ("Windows chronił Twój komputer") — to normalne dla mniejszych, niezależnych aplikacji bez płatnego certyfikatu podpisu. Kliknij **"Więcej informacji" → "Uruchom mimo to"**.
4. Gotowe — aplikacja Cię poprowadzi.
