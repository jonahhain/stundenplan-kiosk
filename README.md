# Stundenplan Kiosk

Eine bessere Lösung, um den Stundenplan im Foyer anzuzeigen.

## Überblick

Dieses Skript richtet ein Debian-System ein, sodass es automatisch Firefox im Kiosk-Modus mit meiner Webseite startet. Ermöglicht wird dies mithilfe von [Cage](https://github.com/cage-kiosk/cage).

Die Webseite ist übrigens [hier](https://jonahhain.github.io/stundenplan) zu finden.

## Installation

1. Laden Sie die [Debian Netinstall ISO](https://www.debian.org/CD/netinst/) herunter.

2. Schreiben Sie das Image mithilfe von [Balena Etcher](https://etcher.balena.io/) auf einen USB-Stick. Stecken Sie diesen anschließend in das Zielgerät und starten Sie es. Alternativ kann eine virtuelle Maschine verwendet werden.

3. Folgen Sie dem Installationsprozess. Für eine Anleitung bitte [hier](https://youtu.be/WbAbyGPm8IA) entlang.

    **Wichtig**: Bei der Softwareauswahl nur "SSH Server" und "Standard-Systemwerkzeuge" auswählen (keine Desktop-Umgebung!)

4. Führen Sie das Skript aus:

    ```bash
    sudo sh -c 'wget -qO- https://raw.githubusercontent.com/jonahhain/stundenplan-kiosk/main/setup_kiosk | bash'
    ```

5. Nach Abschluss das System neu starten:
   ```bash
   sudo reboot
   ```