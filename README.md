# Ultimativer Wii Modding Guide

# Was ihr braucht

1. Eine Wii (nicht die Wii Mini)
2. Eine SD-Karte (mindestens 4GB)
3. Einen PC oder Laptop, um Daten auf der SD-Karte zu bearbeiten

# SD Karten Vorbereitung

## Windows:

Um die SD-Karte auf `Fat32` zu formatieren, führe die folgenden Schritte aus:

1. Rechtsklicke auf die SD-Karte und wähle `Formatieren`.
2. Wähle als Dateisystem `Fat32` aus und klicke auf `Formatieren`. 
   
   **Hinweis:** Wenn "Fat32" nicht als Option angezeigt wird, öffne die Eingabeaufforderung (cmd) als Administrator und führe die folgenden Befehle aus:

   ```sh
   diskpart
   list disk
   sel disk 2   // Wähle die Nummer der SD-Karte, z.B. Disk 2
   format fs=fat32 quick

Falls du eine SD-Karte hast, die größer als 32 GB ist und deine Wii sie nicht erkennt, lade das Programm "Fat32 Format" herunter (von beliebiger Quelle). Wähle deine SD-Karte aus und setze die Größe auf 32768, um sie auf 32 GB zu begrenzen.

## Linux:

Um die SD-Karte in Linux zu formatieren, führe diese Schritte aus:

1. Öffne das Terminal und führe `lsblk` aus, um die Disk-Informationen zu erhalten.
2. Wähle die SD-Karte aus, indem du `sudo fdisk /dev/disk1` eingibst (ersetze `disk1` durch den tatsächlichen Namen der SD-Karte)
3. Führe diesen Befehl aus, um die Partition in FAT32 zu formatieren:

   ```bash
   sudo mkfs.vfat -F 32 /dev/disk1

## MacOS:

Um in MacOS die SD-Karte in FAT32 zu formatieren, führe diese Schritte aus:

1. Öffne das Terminal und schreibe `diskutil list`, um die Infos für die Disk zu bekommen.
2. Unmounte die SD-Karte zuerst mit `diskutil unmountDisk /dev/disk1` (ersetze `disk1` durch den tatsächlichen Namen der SD-Karte).
3. Führe dann den Befehl aus, um die SD-Karte in FAT32 zu formatieren: `diskutil eraseDisk FAT32 namedersdkarte MBRFormat /dev/disk1`.

# Wii Vorbereitung

1. Gehe auf deiner Wii unten rechts im Home-Menü auf "Wii-Optionen".
2. Wähle "Wii-Einstellungen".
3. Scrolle nach rechts auf "Internet".
4. Gehe dann auf "Konsolen-Information".
5. Merke dir die "MAC-Adresse" der Internetverbindung, die du gerade benutzt, und teile sie mit niemandem, dem du nicht vertraust.
6. Packe die SD-Karte in deinen PC.

# SD-Karten Setup

1. Gehe auf die Webseite von Letterbomb [letterbomb](https://please.hackmii.com/)
2. Gib deine "MAC-Adresse" dort ein.
3. Stelle sicher, dass deine Konsolen-Version stimmt (U: NTSC-U, E: PAL/Europäisch, J: Japanisch, K: Koreanisch).
4. Wähle dann die richtige Version aus und stelle sicher, dass der Haken bei `Bundle the HackMii Installer for me!` gesetzt ist.
5. Klicke dann auf `Cut the red wire` oder `Cut the blue wire` (beide Optionen machen das Gleiche).
6. Ziehe nun den `private`-Ordner und die `boot.elf`-Datei auf das Stammverzeichnis der SD-Karte.
7. Packe die SD-Karte wieder in deine Wii.

# Payload Laden

1. Gehe auf deiner Wii unten rechts auf das "Wii Message Board".
2. Scrolle ein bisschen nach links und rechts, bis du einen Brief mit einer Bombe findest.
3. Wähle den Brief mit der Bombe aus und warte.
4. Im `HackMii Installer` wähle "Continue" aus und dann "Install the Homebrew Channel" und wähle "Yes, continue".
5. Wähle dann "Continue" und dann "Exit", um in den Homebrew Launcher zu starten.
