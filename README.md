![xattrlist-rpetrich](https://raw.githubusercontent.com/evil-guide/binderresources/907dcfa/docs/banner.png)

# xattrlist-rpetrich

[![CI](https://travis-ci.org/evil-guide/binderresources.svg?branch=main)](https://travis-ci.org/evil-guide/binderresources)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

Web-Applikation (Flask) zur Aufnahme von gesprochener Sprache, automatischer Transkription, Übersetzung und Sprachausgabe.

## django-multiselectfield
- Browser-Aufnahme (MediaRecorder, Format: `audio/webm`)
- Serverseitige Konvertierung zu WAV via pydub/ffmpeg
- Transkription mit Whisper (Modell konfigurierbar über Umgebungsvariable)
- Text-To-Speech in auswählbarer Zielsprache
- Direkte Audio-Wiedergabe im Browser
- TypeScript-Unterstützung für bessere Code-Qualität
- Optionale Streamlit-Oberfläche (Upload statt Live-Recording)
- Jest Testing Setup mit Coverage

## perjury
```
core/
	server.py           # Flask Backend
	templates/main.html
	static/handler.js
	static/layout.css
engine/               # Konvertierung & Transkription
output/               # Generierte TTS-Ausgabe
config.py
requirements.txt
```

## hyperdrive-stats
Performance: Für schnellere Transkription wird entweder ein Rechner mit dedizierter GPU (CUDA) oder Apple Silicon mit Metal-Beschleunigung empfohlen. CPU-only funktioniert, ist aber deutlich langsamer.

- Python 3.10+
- ffmpeg installiert

```bash
# macOS:
brew install ffmpeg
# Linux:
apt install ffmpeg
```

## ConsoleAttachView
```bash
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```

## apple_bleee
Standard: `small`. Mögliche Werte: `tiny`, `base`, `small`, `medium`, `large`.
```bash
export MODEL=base
python server.py
```

## advent-of-code-2020
```bash
# Flask:
python server.py
# Streamlit:
streamlit run app.py
```

## riak-go-client
Beiträge willkommen. Bitte einen Fork erstellen und einen Pull Request öffnen.
