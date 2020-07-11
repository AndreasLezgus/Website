# Persönliche Website von Andreas Lezgus
Portfolio: https://www.lezgus.de

NOTE: This README is also available in <a href=https://github.com/AndreasLezgus/Website/blob/master/README_EN.md>English</a>.

Dieses Dokument richtet sich an ein technisches Publikum und stellt den neuesten Stand der Architektur und des Programmcodes meiner Website dar, der möglicherweise noch nicht endgültig ist. Ich freue mich ständig über Hinweise auf Verbesserungen und Ideen, wie die Seiten optimiert werden können.


## Über dieses Projekt
Diese Dokumentation und der Programm-Code wurde von mir eigenständig erstellt und wird als meine persönliche Portfolio Website verwendet. Mein altes Entwickler-Herz versucht immer wieder zu verstehen, wie etwas funktioniert. Ausprobieren, Fehler machen, lernen und verzweifelt nach dem Schreibfehler im Code suchen. Der Bauplan und Source Code dieser Seiten kann von allen kopiert, überprüft, modifiziert und verbessert werden.


## Wer bin ich?
Andreas Lezgus, https://www.lezgus.de/geschichte.html


## Was ist das Ziel diese Projektes?
Diese Portfolio-Seiten sind in der Regel statisch und die Änderungshäufigkeit ist überschaubar gering. Idee des Projektes war es daher, zurück zu den Wurzeln zu gehen.
Einfaches statisches HTML und CSS. Keine Scripting Sprache. Keine Datenbank.
Publizierung auf kostengünstigem Amazon Web Services S3 Speicher mit einfachen CI/CD Werkzeugen zum Testen, Versionieren und Veröffentlichen.
Einsatz eines weltweit verteilten Content Delivery Network (CDN).
Aktualisieren der Seiten mit einem einfachen Texteditor plattformunahängig von jedem Endgerät. Mal sehen, wie weit ich mit diesen einfachen Werkzeugen komme?

Interaktive Inhalte, wie z.B. mein Blog werden durch Verweise auf die jeweilige Plattform lediglich verlinkt.


## Technische Architektur und Prozesse
Meine Website wird auf einem sicheren Amazon Web Service S3 Speicherplatz betrieben. Die statischen HTML-Seiten sind dort schreibgeschützt und nicht öffentlich zugänglich. Die Verteilung und Publikation erfolgt über ein weltweit verteiltes Content Delivery Netzwerk mit Amazon CloudFront über ein HTTPS-Protokoll. Über die Amazon Lambda@Edge Services erfolgen benutzerfreundliche Umleitungen von Kurzbegriffen sowie die automatische Erkennung der Spracheinstellungen des Browsers und Umleitungen auf die jeweilige Sprachversion meiner Webseiten.

Die Veröffentlichungs- und Änderungsprozesse erfolgen über einen Git-Client (ich verwende Atom https://atom.io/ auf dem Mac und WorkingCopy https://workingcopyapp.com/ auf iOS) auf dieses Github Repository. Bei jeder Veränderung dieses Github Repository erfolgt automatisch über Amazon CodePipeline eine Aktualisierung der Website auf dem Amazon S3 Speicher und eine Neuverteilung der Seiten über Amazon CloudFront.


## Datenschutz und Informationssicherheit
Informationen zur Informationssicherheit und zum Datenschutz meiner Portfolio Website sind zu finden unter:
http://www.lezgus.de/transparenz.html


## Urheberrechte
Um eine einfache Möglichkeit einzuräumen für den offenen Zugang und der Vervielfältigung, Bearbeitung und Verbreitung der Inhalte und des Codes verwende ich die Lizenzregelungen der Non-Profit-Organisation <b>Creative Commons</b>. Für die durch mich auf diesen Seiten erstellten Inhalte gelten daher die Lizenzbedingungen des CC-BY (Freie Weiterverbreitung bei Nennung des Autors). Weitere Informationen hierzu findet man in dieser kurzen <a href='https://creativecommons.org/licenses/by/4.0/deed.de'>Zusammenfassung</a>. Soweit die Inhalte auf dieser Seite nicht von mir erstellt wurden, werden die Urheberrechte Dritter beachtet. Insbesondere werden Inhalte Dritter als solche gekennzeichnet. Sollte trotzdem eine Urheberrechtsverletzung auftreten oder keine richtige Kennzeichnung erfolgen, bitte ich um einen entsprechenden Hinweis. Bei Bekanntwerden von möglicherweise Rechtsverletzungen werde ich derartige Inhalte umgehend entfernen. Bitte eine kurze Information senden an: <a href=mailto:info@lezgus.de>info@lezgus.de</a>.


## Danksagungen
Diese Webiste verwendet folgende Frameworks, Code-Bausteine, Grafiken und Symbole.
Allen Autoren danke ich ganz herzlich für Ihre Arbeit, Veröffentlichungen und Unterstützung.

Minimalistic CSS framework von milligram
https://milligram.io/

CSS resets for browsers von normalize
https://necolas.github.io/normalize.css/

Hamburger menü von Håvard Brynjulfsen
https://codepen.io/havardob/pen/zZvLgw

Vector graphics von freepic.com
https://www.freepik.com/free-photos-vectors/

Icons von fontawesome
https://fontawesome.com/

Fonts von Google fonts
https://fonts.google.com/specimen/Open+Sans


---

Herzlichen Dank und beste Grüße aus Steinfurt

Andreas Lezgus

info@lezgus.de
