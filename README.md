# Llama Control

**Llama Control** to darmowa aplikacja na komputer, która pomaga uruchamiać i ogarniać modele AI (takie jak lokalny "ChatGPT") na własnym sprzęcie — bez internetu, bez abonamentu, bez wysyłania niczego na zewnątrz.

## Jak to działa

Modele AI trzymane są lokalnie na Twoim dysku jako pliki. Żeby taki model "ożył" i można było z nim rozmawiać, potrzebny jest silnik, który go uruchomi. Llama Control korzysta z **[llama.cpp](https://github.com/ggml-org/llama.cpp)** — jednego z najpopularniejszych, otwartoźródłowych silników do uruchamiania modeli AI lokalnie.

Llama Control to wygodna **nakładka** na ten silnik:

- **Pilnuje Twoich modeli** — pokazuje listę, ile ważą, kiedy je pobrano, pozwala je oznaczać jako ulubione i opisywać.
- **Sam zainstaluje silnik llama.cpp**, jeśli go jeszcze nie masz — dobiera odpowiednią wersję pod Twoją kartę graficzną.
- **Uruchamia i zatrzymuje model jednym kliknięciem** — bez wpisywania niczego w konsoli.
- **Pozwala pobierać nowe modele** prosto z serwisu HuggingFace (to taki "sklep" z modelami AI) i od razu mówi, czy dany model zmieści się w pamięci Twojej karty graficznej.
- **Sama się aktualizuje**, gdy pojawi się nowa wersja.

Krótko: instalujesz, apka sama dogaduje resztę, Ty tylko klikasz.

### Dlaczego llama.cpp, a nie np. Ollama albo LM Studio?

Bo to nie jest kolejny, osobny silnik AI konkurujący z tamtymi — to celowo **lekka nakładka**, a nie pełna aplikacja. Ollama i LM Studio to swoje własne, kompletne środowiska, które siedzą w tle, zajmują pamięć i zasoby cały czas, nawet gdy nic nie robisz. Llama Control nie ma własnego, ciężkiego silnika działającego w tle — po prostu włącza i wyłącza `llama.cpp` dokładnie wtedy, kiedy chcesz z niego skorzystać, i nie zabiera Ci RAM-u ani mocy komputera, kiedy tego nie robisz.

## Na jakich urządzeniach to działa

- **Obecnie: tylko Windows** (10 lub 11) — komputer stacjonarny lub laptop. Nie działa na telefonach ani tabletach.
- **Karta graficzna NVIDIA (GeForce/RTX) jest zalecana** — wtedy modele AI działają szybko. Bez niej też zadziała, ale wolniej (na samym procesorze).
- Modele AI potrafią ważyć od kilku do kilkudziesięciu gigabajtów, więc warto mieć trochę wolnego miejsca na dysku.

### Plany na przyszłość

- Wsparcie dla **kart graficznych AMD i Intel** (obecnie najlepiej działa z NVIDIA).
- Optymalizacja i wsparcie dla **macOS i Linuksa** (obecnie tylko Windows).

## Jak zacząć

1. Pobierz najnowszy instalator z zakładki **[Releases](../../releases)** po prawej stronie tej strony.
2. Uruchom pobrany plik `.exe`.
3. Windows może pokazać niebieski ekran ostrzegawczy ("Windows chronił Twój komputer") — to normalne dla mniejszych, niezależnych aplikacji bez płatnego certyfikatu podpisu. Kliknij **"Więcej informacji" → "Uruchom mimo to"**.
4. Gotowe — aplikacja Cię poprowadzi.
