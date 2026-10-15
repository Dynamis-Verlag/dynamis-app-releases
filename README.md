# Dynamis App, Direkt-Download

Signierte Android-Builds der Dynamis App, für Geräte ohne Google Play. Gedacht für /e/OS, GrapheneOS, LineageOS und alle, die lieber ohne Store installieren. Hier liegt kein Quellcode, nur die fertigen Dateien.

Die App selbst: [dynamis.vision/app](https://dynamis.vision/app)

## Installation

Die neueste Version steht unter [Releases](https://github.com/Dynamis-Verlag/dynamis-app-releases/releases/latest). Lade die Datei `dynamis-<version>.apk` herunter und öffne sie auf dem Gerät. Android fragt einmalig, ob es Installationen aus dieser Quelle erlauben soll. Das ist der normale Weg, wenn kein Store beteiligt ist.

Die APK enthält alle drei Prozessor-Architekturen, ist deshalb rund 76 MB groß und läuft auf Geräten ab Android 7.

## Vor der Installation lesen

Android behandelt eine hier installierte App und eine aus dem Play Store als zwei verschiedene Installationen, weil sie unterschiedlich signiert sind. Das hat eine Folge, die sich später nicht mehr bequem korrigieren lässt: Die beiden aktualisieren einander nicht. Wer von hier zum Play Store wechseln möchte, muss diese Version vorher deinstallieren, und dabei gehen heruntergeladene Übungen und der lokale Fortschritt verloren. Der Account und alles, was am Account hängt, bleiben erhalten.

Solange die App in der Beta ist, können Kontodaten zwischen Versionen zurückgesetzt werden. Das gilt für alle Kanäle gleichermaßen, hier wie im offenen Test bei Google Play und TestFlight.

## Datei prüfen

Zu jeder APK liegt eine Datei `.sha256` mit der Prüfsumme daneben:

```
shasum -a 256 dynamis-1.0.0-26.apk
```

Die Ausgabe muss mit dem Inhalt der `.sha256`-Datei übereinstimmen.

## Updates mit Obtainium

Ohne Store gibt es keine automatischen Updates. [Obtainium](https://obtainium.imranr.dev/) schließt diese Lücke: Es beobachtet dieses Repository und meldet sich, sobald eine neue Version erscheint.

Nach der Installation von Obtainium genügt ein Tippen auf diesen Link auf dem Telefon:

[Dynamis in Obtainium hinzufügen](https://apps.obtainium.imranr.dev/redirect?r=obtainium://app/%7B%22id%22%3A%22ch.dynamis.app%22%2C%22url%22%3A%22https%3A%2F%2Fgithub.com%2FDynamis-Verlag%2Fdynamis-app-releases%22%2C%22author%22%3A%22Dynamis%20Seminare%20%26%20Verlag%22%2C%22name%22%3A%22Dynamis%22%7D)

Von Hand geht es genauso: In Obtainium »App hinzufügen« öffnen und diese Adresse einsetzen.

```
https://github.com/Dynamis-Verlag/dynamis-app-releases
```

## /e/OS App Lounge

Wer /e/OS nutzt, braucht diesen Weg nicht dauerhaft. Die App Lounge bezieht Apps aus dem Play-Katalog, die Dynamis App erscheint dort also von selbst, sobald sie im Play Store öffentlich verfügbar ist. Bis dahin ist der Direkt-Download der schnellere Weg.

## Fragen

[info@dynamis.vision](mailto:info@dynamis.vision)

---

© Dynamis. Die App ist urheberrechtlich geschützt, die Dateien hier dürfen unverändert weitergegeben werden.
