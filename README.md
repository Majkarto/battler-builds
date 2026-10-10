9# Battler – buildy testowe

Pobieranie: **[najnowsze wydanie (Releases)](https://github.com/Majkarto/battler-builds/releases/latest)** – plik `..._linux.zip` dla Linuksa, drugi zip dla Windowsa. Wszyscy gracze muszą mieć tę samą wersję.


## Znane problemy
- Pierwsze Find game dwóch osób w tej samej sekundzie może utworzyć dwa osobne mecze – wtedy jedna osoba: ESC → Find game ponownie.
- Po wyjściu hosta mecz kończy się dla wszystkich (nie ma przejęcia hosta): pojawi się „Connection to the host lost” → Back to lobby → Find game.
- Dołączyć można tylko do gry z tą samą wersją (lewy dolny róg lobby, prawy dolny róg w bitwie) – wszyscy muszą mieć ten sam zip.
- Balans jednostek jest w trakcie prac (łucznicy, trolle, morale), drzewka jednostek się jeszcze zmienią.
- Znane błędy balansu (stan 2026-10-10): łucznicy elfów potrafią wystrzelać rycerzy; pikinierzy zaatakowani konnicą z boku czasem wygrywają; rycerze wygrywają długą walkę z miecznikami; katapulta słabo rani trolle.
- Linux: rozpakuj zip, `chmod +x Battler.x86_64`, uruchom `./Battler.x86_64` (Steam nie jest wymagany; Find game działa między Windows i Linux, jeśli wersja w rogu jest ta sama).
- Teksty są po angielsku.
- Przy bardzo dużych bitwach FPS hosta może spadać.
