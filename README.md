# NB Flow

NB Flow er en gratis app for macOS som gjør tale om til tekst og limer teksten inn der markøren står. Den ligger i menylinjen: hold inne en tast, snakk, og slipp.

Talegjenkjenningen kjører **helt lokalt på Macen** med [NB-Whisper](https://huggingface.co/NbAiLab) fra Nasjonalbiblioteket. Lyden sendes ikke noe sted, og appen trenger ingen konto eller API-nøkkel.

**[⬇︎ Last ned siste versjon (NBFlow.zip)](https://github.com/andreassolberg/nbflow/releases/latest/download/NBFlow.zip)** · [Alle versjoner](https://github.com/andreassolberg/nbflow/releases)

## Krav

- macOS 14 Sonoma eller nyere
- Mac med Apple Silicon (M1 eller nyere)
- Ca. 1 GB ledig minne mens appen kjører

## Installasjon

1. Last ned **NBFlow.zip** og dobbeltklikk for å pakke den ut.
2. Flytt **NB Flow** til mappen Programmer.
3. Åpne NB Flow. Første gang sier macOS at appen ikke kan åpnes, fordi den ikke er notarisert av Apple. Trykk **Ferdig**.
4. Gå til **Systeminnstillinger › Personvern og sikkerhet**, bla ned til Sikkerhet og trykk **Åpne likevel** ved NB Flow. Bekreft med passordet ditt.
5. Gi NB Flow tilgang til **mikrofonen**, og under **Tilgjengelighet** (Personvern og sikkerhet), slik at appen kan lime inn tekst og bruke enkelttaster.

Steg 3 og 4 trengs bare første gang.

## Bruk

| Handling | Standard |
|---|---|
| Hold inne for å snakke | Høyre `⌘ Command` |
| Start og stopp opptak | `⌃⌥⇧Space` |
| Avbryt et opptak | `Esc` |

Tastene kan endres under Innstillinger. Når du stopper, limes teksten inn i feltet du står i, eller den legges i utklippstavlen.

## Modeller

| Modell | Størrelse | Svartid* |
|---|---|---|
| NB-Whisper Turbo (standard, følger med) | 0,5 GB | 0,3–0,7 s |
| NB-Whisper Large (kan lastes ned i appen) | 1,1 GB | 0,6–1,7 s |

\* Fra du slipper tasten til teksten er klar, for setninger på 3–12 sekunder, målt på en MacBook med M2.

NB-Whisper skriver bokmål, nynorsk eller engelsk, og forstår norske dialekter.

## Personvern

All talegjenkjenning skjer på maskinen. NB Flow sender ikke lyd eller tekst ut, og samler ikke inn noe. Appen kobler seg bare til internett hvis du selv laster ned Large-modellen fra Hugging Face.

## Vilkår

NB Flow er gratis å laste ned og bruke. Kildekoden er ikke offentlig. Appen leveres som den er, uten garantier.

NB Flow bruker [NB-Whisper](https://huggingface.co/NbAiLab) fra Nasjonalbiblioteket (Apache 2.0) og [whisper.cpp](https://github.com/ggml-org/whisper.cpp) (MIT). Lisenstekstene ligger i appen under Innstillinger › Modell › Vis lisenser.

Spørsmål og feil kan meldes under [Issues](https://github.com/andreassolberg/nbflow/issues).
