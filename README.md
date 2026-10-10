# Battler

Bitwy oddziałów w klimacie fantasy. Dowodzisz trzema oddziałami i razem z drużyną walczysz o wzgórze na środku mapy. To wczesna wersja testowa.

## Pobierz

| System | Plik |
|---|---|
| Windows | [Battler_0.1.0_c53e1fc_windows.zip](https://github.com/Majkarto/battler-builds/releases/download/v0.1.0-c53e1fc/Battler_0.1.0_c53e1fc_windows.zip) |
| Linux | [Battler_0.1.0_c53e1fc_linux.zip](https://github.com/Majkarto/battler-builds/releases/download/v0.1.0-c53e1fc/Battler_0.1.0_c53e1fc_linux.zip) |

Windows i Linux grają razem, ale wszyscy muszą mieć tę samą wersję.

## Uruchomienie

**Windows:** rozpakuj zip i odpal `battler.exe`. Gdy Windows zaprotestuje, kliknij „Więcej informacji”, potem „Uruchom mimo to”.

**Linux:** rozpakuj zip, potem `chmod +x Battler.x86_64` i `./Battler.x86_64`.

W lobby wybierz oddziały i kliknij **Find game**. Jeśli nikt akurat nie gra, gra sama założy mecz i dobierze boty.

## Sterowanie

| Klawisz | Co robi |
|---|---|
| LPM | wybór oddziału |
| PPM | ruch, a na wrogu atak |
| WASD, Q/E, kółko | kamera |
| 1 / 2 / 3 | podmiana oddziału |
| F / R | formacja / sprint |
| H / V / L | łucznicy: wstrzymaj ogień / salwa / stromy tor |
| F8 | zapis raportu z błędu (trafia do `Dokumenty\Battler Reports`) |

## Znane problemy

- Gdy host wyjdzie, mecz kończy się wszystkim.
- Dwie osoby klikające Find game w tej samej sekundzie mogą założyć dwa osobne mecze. Jedna niech poszuka jeszcze raz.
- Balans jest w trakcie prac, np. łucznicy elfów są za mocni na konnicę.
- Teksty w grze są po angielsku.
