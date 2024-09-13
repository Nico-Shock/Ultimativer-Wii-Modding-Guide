# Ultimativer Wii Modding Guide

# Was ihr braucht

1. Eine Wii (nicht die Wii Mini)
2. Eine SD Karte (mindestens 4GB)
3. Einen PC oder Laptop, um Daten auf der SD Karte zu bearbeiten

# SD Karten Vorbereitung

## Windows

1. Ladet euch [Fat32 Format](http://ridgecrop.co.uk/index.htm?guiformat.htm) herunter.
2. Startet die "guiformat.exe".
3. Wählt eure SD Karte aus (z.B. "D:").
4. Falls eure SD Karte 32 GB oder mehr hat, wählt "32768" bei "allocated unit size" aus, damit eure Wii die SD Karte erkennen kann. (Manche SD Karten, insbesondere ältere, könnten trotzdem nicht erkannt werden, wenn sie größer als 32 GB sind.)

## MacOS

1. Startet das "Festplattendienstprogramm".
2. Rechtsklickt auf die SD Karte und wählt dann "Löschen" aus. Formatiert sie als Fat32 (es wird eventuell als "MS-DOS-Dateisystem" angezeigt).
3. Wählt anschließend "Löschen".

## Linux

1. Öffnet die "Disk" App.
2. Wählt die Festplatte aus, klickt dann auf das Zahnradsymbol oder macht einen Rechtsklick und wählt "Formatieren".
3. Wählt beim Typ "Fat32" aus (eventuell müsst ihr unter "Other" oder "Weitere" nach Fat32 suchen).

# Wii Vorbereitung

1. Gehe auf deiner Wii unten rechts im Home Menü auf "Wii Optionen".
2. Wähle "Wii Einstellungen".
3. Scrolle nach rechts auf "Internet".
4. Gehe dann auf "Konsolen Information".
5. Merke dir die "MAC Adresse" der Internetverbindung, die du gerade benutzt, und teile sie mit niemandem, dem du nicht vertraust.
6. Packe die SD Karte in deinen PC.

# SD Karten Setup

1. Gehe auf die Webseite von Letterbomb [letterbomb](https://please.hackmii.com/)
2. Gib deine "MAC Adresse" dort ein.
3. Stelle sicher, dass deine Konsolen Version stimmt (U: NTSC-U, E: PAL/Europäisch, J: Japanisch, K: Koreanisch).
4. Wähle dann die richtige Version aus und stelle sicher, dass der Haken bei `Bundle the HackMii Installer for me!` gesetzt ist.
5. Klicke dann auf `Cut the red wire` oder `Cut the blue wire` (beide Optionen machen das Gleiche).
6. Ziehe nun den `private` Ordner und die `boot.elf` Datei auf das Stammverzeichnis der SD Karte.
7. Packe die SD Karte wieder in deine Wii.

# Payload Laden

1. Gehe auf deiner Wii unten rechts auf das "Wii Message Board".
2. Scrolle ein bisschen nach links und rechts, bis du einen Brief mit einer Bombe findest.
3. Wähle den Brief mit der Bombe aus und warte.
4. Im `HackMii Installer` wähle "Continue" aus und dann "Install the Homebrew Channel" und wähle "Yes, continue".
5. Wähle dann "Continue" und dann "Exit", um in den Homebrew Launcher zu starten.
