# Mobile Music Studio (Android-fähige PWA)

## Enthaltene Funktionen
- 8-Takt-Timeline mit mehreren Spuren
- Touch-MIDI/Drum-Step-Editor
- Web-Audio-Synthesizer für Drumhits, Bass, Keys und Gitarren-Synth
- BPM-Steuerung, Wiedergabe, Mute/Solo, Lautstärke und Panorama
- Mikrofonaufnahme über MediaRecorder (WebM)
- WAV-Export der programmierten MIDI-Spuren
- Projektdatei als JSON
- Offline-Cache und PWA-Manifest

## Auf Android installieren
Die Installation als App erfordert eine HTTPS-Adresse (oder localhost). Am einfachsten:
1. Entpacke den ZIP-Ordner auf einem PC.
2. Lade die Dateien in ein neues GitHub-Repository hoch.
3. Öffne im Repository **Settings → Pages**.
4. Wähle **Deploy from a branch**, Branch `main`, Ordner `/ (root)` und speichere.
5. Öffne die angezeigte HTTPS-Adresse in Chrome auf Android.
6. Wähle im Chrome-Menü **App installieren** oder **Zum Startbildschirm hinzufügen**.

Alternativ kann der Ordner auf einen beliebigen HTTPS-Webhost geladen werden.

## Hinweise
Dies ist eine erste lauffähige Web-App, keine native APK. Die Audio-Engine verwendet synthetisch erzeugte Sounds, keine hochwertigen gesampelten Instrumentenbibliotheken. Die Mikrofonaufnahme wird als WebM gespeichert und ist getrennt vom MIDI/WAV-Mix. Der WAV-Export rendert die programmierten MIDI-Spuren. Echte Audio-Spuren sind derzeit noch nicht in den WAV-Mix integriert. Für Mikrofonzugriff muss die App über HTTPS geöffnet werden.

Für eine native Android-APK ist anschließend ein Android-Studio/Capacitor-Build nötig.
