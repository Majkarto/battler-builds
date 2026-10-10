# Battler – buildy testowe

Pobieranie: **[najnowsze wydanie (Releases)](https://github.com/Majkarto/battler-builds/releases/latest)** – plik `..._linux.zip` dla Linuksa, drugi zip dla Windowsa. Wszyscy gracze muszą mieć tę samą wersję.

---

# Battler – instrukcja dla testerów (sobota 2026-10-10, 16:00)

Dzięki za pomoc! Gra jest we wczesnej wersji: będą błędy, prosimy o raporty (F8).

## Start
1. Pobierz zip z linku od organizatora, rozpakuj go w dowolne miejsce (np. na Pulpit). **Nie uruchamiaj exe z wnętrza zipa.**
2. Uruchom `Battler/Battler.exe`. Windows może pokazać „System Windows ochronił ten komputer” → **Więcej informacji → Uruchom mimo to** (gra nie ma podpisu cyfrowego).
3. Zapora sieciowa może zapytać o dostęp – zezwól (sieci prywatne i publiczne).
4. Przy pierwszym uruchomieniu gra tworzy Twój profil (złoto, badania, oddziały). **Reset profile** na dole lobby zaczyna od zera.

## Lobby
- Zakładki ras na górze, drzewko jednostek: **Research** (badanie XP) i **Buy** (złoto).
- Dodaj do 3 oddziałów jednej rasy do **lineupu** (pasek na dole).
- **Find game** – gra szuka otwartego meczu i dołącza; jeśli żadnego nie ma, sama go zakłada i czeka na innych (w meczu walczą też boty, ludzie zastępują boty). **Cancel** przerywa szukanie.
- **Battle!** – mecz tylko z botami (na rozgrzewkę).
- **Advanced ▾ → Host by code / Join** – awaryjnie, gdy Find game nie działa: jedna osoba hostuje i podaje kod z ekranu, druga go wpisuje.

## Sterowanie w bitwie
| Klawisz | Działanie |
|---|---|
| LPM | wybór oddziału |
| PPM na ziemi (przeciągnij = szerokość frontu) | ruch |
| PPM na wroga | atak / ostrzał |
| W A S D, Q E, kółko myszy | kamera |
| 1 / 2 / 3 | zmiana oddziału (powrót na tyły i wystawienie innego), C – anuluj |
| F | formacja |
| R | sprint |
| H | wstrzymaj ogień, V – salwa / ogień dowolny, L – stromy tor strzału |
| ESC | wyjście z meczu (liczy się jako porażka) |
| **F8** | **zapisz raport** |

Cel meczu: utrzymać wzgórze (Król Wzgórza) – punkty rosną, gdy na szczycie jest tylko Twoja drużyna.

## Raport z błędem (F8)
Gdy coś pójdzie nie tak (dziwne zachowanie, przycięcie, rozłączenie) – **od razu naciśnij F8**. Na ekranie pojawi się ścieżka, zwykle
`Dokumenty\Battler Reports\battler_report_<data>.zip`. Wyślij ten plik organizatorowi z jednym zdaniem: co robiłeś i co się stało.
Gdy gra się wysypie: uruchom ją ponownie i naciśnij F8 w lobby (raport zawiera też log poprzedniego uruchomienia).

## Co sprawdzamy (zaznacz, co udało się zrobić)
- [ ] Find game: dołączenie do meczu innej osoby
- [ ] Find game, gdy nikt nie gra: założenie meczu i dołączenie kogoś do Ciebie
- [ ] Rozkazy: ruch, atak, formacja, sprint, zmiana oddziału 1/2/3
- [ ] Łucznicy: ostrzał, H / V / L
- [ ] Mecz do końca: ekran wyniku → Back to lobby → nagrody w profilu (złoto, XP)
- [ ] Drugi mecz po powrocie do lobby
- [ ] Wyjście z meczu (ESC) i ponowne Find game
- [ ] Lag: czy jednostki „skaczą”, opóźnienie rozkazów (HUD pokazuje RTT)
- [ ] F8 działa

## Znane problemy
- Pierwsze Find game dwóch osób w tej samej sekundzie może utworzyć dwa osobne mecze – wtedy jedna osoba: ESC → Find game ponownie.
- Po wyjściu hosta mecz kończy się dla wszystkich (nie ma przejęcia hosta): pojawi się „Connection to the host lost” → Back to lobby → Find game.
- Dołączyć można tylko do gry z tą samą wersją (lewy dolny róg lobby, prawy dolny róg w bitwie) – wszyscy muszą mieć ten sam zip.
- Balans jednostek jest w trakcie prac (łucznicy, trolle, morale), drzewka jednostek się jeszcze zmienią.
- Znane błędy balansu (stan 2026-10-10): łucznicy elfów potrafią wystrzelać rycerzy; pikinierzy zaatakowani konnicą z boku czasem wygrywają; rycerze wygrywają długą walkę z miecznikami; katapulta słabo rani trolle.
- Linux: rozpakuj zip, `chmod +x Battler.x86_64`, uruchom `./Battler.x86_64` (Steam nie jest wymagany; Find game działa między Windows i Linux, jeśli wersja w rogu jest ta sama).
- Teksty są po angielsku.
- Przy bardzo dużych bitwach FPS hosta może spadać.
