# Änderungsprotokoll

Alle bemerkenswerten Änderungen an diesem Projekt werden in dieser Datei dokumentiert.

Dieses Projekt hält sich an [Semantic Versioning](https://semver.org/).

## [2.9.0] - 2024-09-15
- **Tabs löschen** hinzugefügt: Speichern Sie einen Schnappschuss und schließen Sie alle Tabs außer dem aktiven. Stellen Sie sie aus kürzlich geschlossenen Tabs oder Schnappschüssen wieder her.
- **Automatische Aktivierung der Tab-Gruppierung** hinzugefügt: Erstellen Sie automatisch eine neue Gruppe, wenn Sie einen neuen Tab öffnen. Nachfolgende Tabs, die von diesem Tab geöffnet werden, treten der Gruppe bei.
- **Vertikaler Abstand der Liste** hinzugefügt: Neue Option in den erweiterten Tab-Gruppeneinstellungen, um den vertikalen Abstand für Listenelemente anzupassen.
- **Mehrere URLs zum Schnellzugriff hinzufügen** hinzugefügt: Ermöglicht das Hinzufügen von Gruppen und das Auswählen mehrerer Tabs, die im Schnellzugriff gespeichert werden sollen.
- **Abstand der Schnellzugriffselemente** hinzugefügt: Legen Sie den vertikalen/horizontalen Abstand für Schnellzugriffselemente auf der Optionsseite fest.

---
## [2.8.0] - 2024-09-12

### Hinzugefügt
- **Tab-Verlauf** hinzugefügt: Jetzt können Sie leicht sehen, welche Websites unter demselben Tab geöffnet wurden. Linksklick, um die Website im aktuellen Tab zu öffnen, Mittelklick oder Strg+Linksklick, um die Website in einem neuen Tab zu öffnen. Weitere Details finden Sie auf der Optionsseite.
- **Benutzerdefinierte Gruppennamen** hinzugefügt: Auf der Optionsseite - Erweitertes Tab-Gruppe, können Sie hier einige vordefinierte Gruppen hinzufügen, sodass Sie diese schnell auswählen können, wenn Sie Tabs zu einer Gruppe hinzufügen müssen. Wir haben bereits einige Gruppennamen voreingestellt, die Sie nach Bedarf ändern oder löschen können.
- **Verwenden Sie den Lesezeichenordnernamen als Gruppennamen** hinzugefügt: Auf der Optionsseite - Erweitertes Tab-Gruppe wurde eine neue Option hinzugefügt. Wenn die geöffnete Website ein Lesezeichen ist, wird sie automatisch der Gruppe hinzugefügt, und der Gruppenname verwendet den Lesezeichendirectorynamen.
- **Tab-Index** hinzugefügt: Auf der Optionsseite, wenn aktiviert, wird der Tab-Index neben dem Titel angezeigt, was es einfach macht, den aktiven Tab mit [Strg+Nummer] unter Windows oder [cmd+Nummer] auf dem Mac zu aktivieren. Beispiel: 1. stackoverflow.com 2. youtube, sodass es einfach ist, Strg + 2 unter Windows oder cmd + 2 auf dem Mac zu verwenden, um zu youtube zu gelangen.
- **Optimierte Seiteneinstellungen**: Verbesserte Option zum Festlegen der Hintergrundfarbe und Schriftfarbe für Websites.

### Geändert
- Beim Überprüfen von Lesezeichen das Aktualisieren von umgeleiteten URLs zulassen. Wenn die URL nicht zugänglich ist, Fehlercodes anzeigen: Erfolgreiche Antworten (200 – 299), Umleitungsnachrichten (300 – 399), Client-Fehlerantworten (400 – 499), Server-Fehlerantworten (500 – 599). Weitere Details finden Sie unter: https://developer.mozilla.org/en-US/docs/Web/HTTP/Status

### Behoben
- Das Problem behoben, bei dem das Popup zur Lesezeichenänderung nicht verschwand

---

## [2.7.0] - 2024-09-05
### Hinzugefügt
- **Lesezeichenverwaltung** hinzugefügt: Voll funktionsfähige Lesezeichenverwaltungsfunktion hinzugefügt
- **Tab-Navigationsleiste** hinzugefügt: Optionen im Erscheinungsbild, Anzeige: Tabs, Lesezeichen, Verlauf, kürzlich geschlossene Tabs, Leseliste und Schnellzugriff im Seitenbereich
- **Tab zu Gruppe hinzufügen** Menü hinzugefügt: Tabs zu einer neuen Gruppe oder einer bestehenden Gruppe hinzufügen
- Suchbegriff-Hervorhebung hinzugefügt
- Premium-Edition-Reservierung hinzugefügt
### Geändert
- Cookie-, Leselisten- und Lesezeichenberechtigungen zu optionalen Berechtigungen angepasst, die eine Benutzerautorisierung erfordern
### Veraltet
- **Optionen-Seite - Verlauf - Im Seitenbereich anzeigen**: Diese Option wurde durch die *Tab-Navigationsleiste* ersetzt und wird bald veraltet sein

### Behoben
- Das Problem behoben, bei dem die Schaltfläche zum Erweitern der Gruppe beim ersten Klicken auf die Seitenleiste nicht angezeigt wurde
- Das Problem behoben, bei dem nach dem Neustart des Browsers und dem Klicken auf das Erweiterungssymbol eine erneute Auswahl zwischen Popup oder Seitenleiste erforderlich war
- Das Problem behoben, bei dem die Größen des angehefteten Tab-Symbols und des Schnellzugriffssymbols inkonsistent waren

---

## [2.6.1] - 2024-08-30

### Geändert
- Menüanzeigemethode optimiert, Fehlermeldungen verbessert
- Mehr Kompatibilität für Chromium-basierte Browser hinzugefügt


---

## [2.6.0] - 2024-08-28
### Hinzugefügt
- **Tab-Menü-Zoom** hinzugefügt: Eine Zoomfunktion wurde dem Tab-Menü hinzugefügt, mit der Sie den Zoomlevel frei von 1% bis 1000% anpassen können.

### Geändert
- Schnellzugriff wurde in ein separates Menüelement verschoben.
- Drag-and-Drop-Sortierung optimiert

### Behoben
- Ein Problem behoben, bei dem einige Bereiche nach dem Ändern der Schriftfarbe nicht geändert wurden.

### Veraltet
- **Schnellzugriff im Tab-Menü**: Schnellzugriff wurde in ein separates Menüelement verschoben. Die Option im Tab-Menü wird bald veraltet sein (die Funktionalität bleibt gleich).

### Entfernt
- Die Zoomoption aus den Seiteneinstellungen entfernt, da das Anpassen des Zooms im Menü keine intuitive Vorschau der Änderungen bot. Die Zoomfunktion wurde in das Tab-Menü verschoben, um eine Echtzeitvorschau zu ermöglichen.

---

## [2.5.2] - 2024-08-27

### Behoben

- Das Problem behoben, bei dem gespeicherte Hintergrundbilder nach dem Neustart der Anwendung verloren gingen
- Das Problem behoben, bei dem das Schließen aller Tabs derselben Seite in allen Fenstern fehlschlug
- Absturz beim Deaktivieren von DnD behoben

------

## [2.5.0] - 2024-08-25

### Hinzugefügt

- Unterstützung für Drag-and-Drop-Sortierung von Tabs und Gruppen in der Tab-Reihenfolge und Synchronisierung mit Chrome
- Synchronisierung des Gruppen-Erweiterungszustands mit Chrome

### Behoben
- Das Problem behoben, bei dem das Hochladen einer zu großen Hintergrundbilddatei einen QUOTA_BYTES-Quota-Überschreitungsfehler verursachte
- Das Problem behoben, bei dem das Anzeigen aller Fenster-Tabs einen Fehler verursachte und die Gruppierung nach Seite fehlschlug


---

## [2.4.0] - 2024-08-20

### Hinzugefügt
- **Hintergrundbild hochladen** hinzugefügt: Sie können ein Bild von Ihrem lokalen Gerät hochladen, um es als Hintergrund zu verwenden.
- **Benutzerdefinierte Hintergrundfarbe** hinzugefügt: Unterstützt jetzt benutzerdefinierte Hintergrundfarben, und Sie können auch eine Farbe auswählen, um einen schönen Farbverlauf zu erzeugen

### Geändert

- **Schriftfarbe**: Die Schriftfarbe ändert sich automatisch zu Schwarz oder Weiß basierend auf der dominanten Farbe des Hintergrunds oder Hintergrundbilds. Wenn das Bild groß ist, kann es einige Zeit dauern, bis der Hintergrund angewendet wird, was normal ist.

### Behoben
- Das Problem behoben, bei dem einige Bereiche nach dem Ändern der Schriftfarbe nicht geändert wurden

### Veraltet
- **Listenhintergrundstil**: Diese Funktion legt den Hintergrundstil für jede Liste fest, mit einigen eingebauten Farbverläufen. Mit der Veröffentlichung benutzerdefinierter Hintergrundfarben ist ihre Aufgabe jedoch abgeschlossen und sie wird bald entfernt.

---

## [2.3.0] - 2024-08-16

### Hinzugefügt
- **Seitenleiste auf Seiten** hinzugefügt: Die Seitenleiste ermöglicht es Ihnen, eine Seitenleiste in die von Ihnen durchsuchten Webseiten einzufügen, ohne die Browser-Seitenleiste zu öffnen, um Tabs zu verwalten. Dies ist eine sehr nützliche Funktion für Benutzer mit kleineren Bildschirmauflösungen, die die Browser-Seitenleiste als zu breit und nicht anpassbar empfinden. Aufgrund einiger Einschränkungen bietet die Seitenleiste jedoch nur sehr begrenzte Funktionalität. Wenn diese Funktion aktiviert ist, können Sie die Maus verwenden, um über den Rand des Fensters zu fahren, um die Seitenleiste herauszubringen.

### Entfernt
- **Schwebender Ball** entfernt

---

## [2.2.0] - 2024-08-14

### Hinzugefügt
- Neues Tab-Menü **Tab aktiv halten**: Halten Sie den Tab aktiv, damit er nicht automatisch verworfen wird.

### Geändert
- Leistung optimiert und Paketgröße reduziert.

---

## [2.1.0] - 2024-08-10

### Hinzugefügt
- Fenster-, Gruppen- und Tab-Snapshots automatisch speichern. Nach dem Neustart des Browsers, wenn nur ein Fenster geöffnet ist und weniger als 5 neue Tabs geöffnet sind, wird ein Toast angezeigt, um das letzte gespeicherte Fenster und die Tab-Informationen wiederherzustellen, wenn die Seitenleiste geöffnet wird.

### Geändert
- Speicherungsdaten für den Schnellzugriff optimiert, um die Zugriffszeit zu verkürzen.

### Behoben
- Andere kleinere Probleme behoben.

---

## [2.0.1] - 2024-08-09

### Behoben
- Das Nachrichtenformat für den erfolgreichen Snapshot-Import behoben.
- Das Problem behoben, bei dem doppelte Importe wiederholte Schnellzugriffseinträge verursachten.

---

## [2.0.0] - 2024-08-08

### Geändert
- Die Erweiterung von "Colorful Side Panel Tabs" in **"VertiTab - Side Panel Vertical Tabs"** umbenannt.

### Hinzugefügt
- Snapshots: Eine Ein-Klick-Speicherfunktion für Browser-Tab-Snapshots hinzugefügt. Sie können Snapshots speichern, bevor Sie den Browser schließen, und sie beim nächsten Öffnen schnell wiederherstellen. Derzeit können bis zu 50 Snapshots gespeichert werden.
- Verbesserte untere Navigationsleiste: Greifen Sie auf mehr Funktionen von der unteren Navigationsleiste zu, wie Lesezeichen, Verlauf, kürzlich geschlossene Tabs, Leseliste, Schnellzugriff, neuen Tab öffnen, Snapshot erstellen, suchen, Gruppen zusammenklappen usw.
- Aktualisierte Import-/Export-Funktionalität: Verbesserte Import- und Exportoptionen, um Tabs besser über Geräte hinweg zu verwalten.

### Behoben
- Fehlerbehebungen und Stabilitätsverbesserungen.

---

## [1.3.3] - 2022-08-04

### Hinzugefügt
- **linkSettings**: Die Seiteneinstellungen enthalten jetzt eine neue Option, mit der Sie Regeln hinzufügen können, um zu steuern, ob Seitenlinks im aktuellen Tab oder in einem neuen Tab geöffnet werden.

---

## [1.3.2] - 2024-08-02

### Behoben
- Das Problem behoben, dass das Klicken auf die mittlere Maustaste zum Schließen des Tabs nicht funktionierte.

---

## [1.3.1] - 2024-08-01

### Geändert
- Das Layout des Schnellzugriffs optimiert und Unterstützung für Drag-and-Drop-Sortierung hinzugefügt.
- Die Logik zum Erweitern aller Gruppen und zum Erinnern ihres Zustands verbessert.

### Behoben
- Das Problem behoben, bei dem das Importieren von Schnellzugriffsdaten fehlschlug, wenn das Seitenpanel nicht geöffnet war.
- Das Problem behoben, bei dem Symbole in der Gruppenansicht falsch ausgerichtet waren.
- Andere kleinere Probleme behoben.

---

## [1.3.0] - 2024-07-30

### Hinzugefügt
- **Import/Export**: Benutzerpräferenzen, Schnellzugriff, Website-Einstellungen und Daten zu kürzlich geschlossenen Tabs exportieren und in einen anderen Browser importieren, um die Erweiterungsdaten zu synchronisieren.
- **Schnellzugriff aus Verlauf auswählen**: Sie können die am häufigsten besuchten Websites aus dem Verlauf durchsuchen und zum Schnellzugriff hinzufügen.
- **Mehr Optionen in der Symbolleiste**: Weitere Optionen zur Symbolleiste hinzufügen. Sie können das Label in der Symbolleiste ausblenden und steuern, welche Symbole in der Symbolleiste angezeigt werden.

### Geändert
- **Suchfeld**: Das Suchfeld unterstützt jetzt die Eingabetaste, um Schlüsselwörter in einem neuen Tab zu suchen. Wenn nach Eingabe des Schlüsselworts keine übereinstimmenden Tabs oder Verlaufsdaten gefunden werden, können Sie die Eingabetaste drücken, um mit der Standardsuchmaschine zu suchen.
- **Dateninitialisierung**: Das Timing der Dateninitialisierung angepasst und wiederholtes Rendern durch Datenänderungen optimiert.
- **Changelog-URL**: Die Changelog-URL auf die Release-URL auf GitHub aktualisiert.
- **Layout-Optimierung**: Layout-Änderungen bei Größenänderung des Fensters optimiert.
- **Fehlerprotokollierung**: Sentry zur Sammlung von Fehlerprotokollen verwenden. Seien Sie versichert, diese Funktion sammelt keine privaten Daten.

### Behoben
- **Tooltip-Positionsfehler**: Das Problem behoben, bei dem das Tooltip beim Wechseln von Themen und Ansichten in der Symbolleiste blinkte.
- **Untere Navigation**: Das Problem behoben, bei dem die untere Navigation die Liste blockierte, wenn viele Tabs geöffnet waren.

---

## [1.2.3] - 2024-07-23

### Behoben
- Falsche Berechnung der Listen-Scrollhöhe behoben, wenn angeheftete Tabs und Schnellzugriffssymbole mehr als eine Reihe überschreiten.

### Geändert
- Inaktive Tabs verwerfen geändert, um angeheftete Tabs auszuschließen.
- Das Schließen aller verworfenen Tabs geändert, um angeheftete Tabs auszuschließen.
- Die Größe der angehefteten und Schnellzugriffssymbole angepasst.

---
## [1.2.2] - 2024-07-19

### Hinzugefügt
- Schnellzugriff hinzufügen: Sie können einen Tab so einstellen, dass er im Schnellzugriff angezeigt wird, damit er leicht zu finden ist. Klicken Sie einfach mit der rechten Maustaste (oder drücken Sie lange) darauf und wählen Sie "An Schnellzugriff anheften". Lösen Sie die Anheftung, wenn Sie ihn dort nicht mehr benötigen, indem Sie mit der rechten Maustaste klicken (oder lange drücken) und "Aus Schnellzugriff löschen" auswählen. Der Unterschied zu angehefteten Tabs besteht darin, dass der Schnellzugriff die URL speichert und jedes Mal einen neuen Tab öffnet, wenn darauf geklickt wird.

### Geändert
- Angeheftete Tabs zeigen nur Symbole an, um zu verhindern, dass sie versehentlich angeklickt und dann gelöst werden.
- Die Größe der angehefteten Tab-Symbole ändern.

---

## [1.2.1] - 2022-07-17

### Hinzugefügt
- Neues Menü zur unteren Navigation hinzufügen: inaktive Tabs verwerfen.
- Neues Menü zur unteren Navigation hinzufügen: alle verworfenen Tabs schließen.

### Geändert
- Änderungen am unteren Navigationsmenü "Nach Website gruppieren" betreffen nur das aktuelle Fenster.

### Behoben
- Das Problem behoben, bei dem die Benutzeroberfläche aufgrund von Höheninkonsistenzen sprang, wenn aktive Tabs in der Liste gewechselt wurden.

---

## [1.2.0] - 2024-07-16

### Hinzugefügt
- Website-Konfigurationen hinzufügen: Passen Sie site-spezifische Einstellungen an, wie z.B. das Deaktivieren des Bild-in-Bild-Modus, das Deaktivieren des automatischen Verwerfungsmodus und mehr.

### Behoben
- Automatisches Erstellen oder Beitreten zu derselben Domain-Gruppe beheben: Ein Problem wurde behoben, bei dem das automatische Erstellen oder Beitreten zu derselben Domain-Gruppe nicht funktionierte, wenn ein Tab aktualisiert wurde.
- Problem beheben, bei dem die Seite keine Konfigurationsaktualisierungsnachrichten empfing: Sicherstellen, dass Seiten Konfigurationsaktualisierungsnachrichten korrekt empfangen.
- Andere Fehler beheben: Verschiedene andere Fehler wurden behoben, um die Stabilität und Leistung zu verbessern.

### Geändert
- Option hinzufügen, um die Schaltfläche zum Schließen bei Hover anzuzeigen: Eine Option wurde hinzugefügt, um die Schaltfläche zum Schließen nur beim Überfahren eines Tabs anzuzeigen.

---

## [1.1.0] - 2024-07-13

### Hinzugefügt
- Leistungsoptionen hinzufügen: Neue Leistungseinstellungen einführen, um Ihr Browser-Erlebnis anzupassen und zu verbessern.
- Zum aktiven Tab-Symbol scrollen hinzufügen: Navigieren Sie einfach zum aktiven Tab mit einem neuen Symbol zum Scrollen zum aktiven Tab.
- Tabs nach Domain sortieren hinzufügen: Organisieren Sie Ihre Tabs nach Domain mit einer neuen Sortierfunktion.
- Alle Tabs stummschalten, die Geräusche machen: Schalten Sie schnell alle Tabs stumm, die Geräusche machen, für ein ruhigeres Browser-Erlebnis.

### Geändert
- Wiederherstellungssymbol entfernen: Das Wiederherstellungssymbol wurde entfernt und durch eine Listentext-Deckkraft von 0,5 für ein saubereres Aussehen ersetzt.

### Veraltet
- Drag-and-Drop-Sortierung entfernen: Die aktuelle Lösung für die Drag-and-Drop-Sortierung hat Leistungsprobleme und wurde vorübergehend entfernt.

---

## [1.0.4] - 2024-07-09

### Hinzugefügt
- Drag-and-Drop-Sortierung für Tabs: Ordnen Sie Ihre Tabs einfach mit der Drag-and-Drop-Funktion neu an.

### Geändert
- Seitenladegeschwindigkeit optimieren: Die Seitenladegeschwindigkeit wurde weiter verbessert, um ein noch reibungsloseres Browser-Erlebnis zu bieten.

---

## [1.0.3] - 2024-07-05

### Behoben
- Fehler im gemischten Ansichtsmenü beheben: Ein Problem wurde behoben, bei dem das gemischte Ansichtsmenü Fehler anzeigte.

### Geändert
- Tab-Gruppen-Domain-Menü optimieren: Das Tab-Gruppen-Domain-Menü wurde verbessert, um eine bessere Organisation und Benutzerfreundlichkeit zu gewährleisten.
- Tab-Padding optimieren: Das Tab-Padding wurde angepasst, um ein schlankeres und visuell ansprechenderes Layout zu erzielen.

---

## [1.0.2] - 2024-07-04

### Hinzugefügt
- Indikator für aktuellen aktiven Tab: Erkennen Sie den aktiven Tab einfach mit einem neuen visuellen Indikator.
- Benutzerdefinierte Schriftfarbe: Personalisieren Sie Ihre Benutzeroberfläche, indem Sie eine benutzerdefinierte Schriftfarbe festlegen.

### Geändert
- Ladegeschwindigkeit optimieren: Die Ladegeschwindigkeit wurde verbessert, um ein schnelleres und reibungsloseres Benutzererlebnis zu bieten.

### Standardeinstellungen
- Standardmäßig keine Farbmodus verwenden: Die Standardeinstellung verwendet jetzt den Einfarbenmodus für ein vereinfachtes Erscheinungsbild.

---

## [1.0.1] - 2024-07-02

### Hinzugefügt
- Vollständige Verlaufserfassung nach Zeitbereich: Greifen Sie auf Ihren Browserverlauf zu und verwalten Sie ihn mit detaillierten Aufzeichnungen, die nach Zeitbereichen sortiert sind.
- Einfarbenmodus für Listen: Ein Einfarbenmodus wurde eingeführt, um ein vereinfachtes und konsistentes Listen-Erscheinungsbild zu bieten.

### Geändert
- Aktualisierungszeitpunkt der vollständigen Audio-Fortschrittsleiste: Die Genauigkeit der Aktualisierungen der Audio-Fortschrittsleiste wurde verbessert, um ein reibungsloseres Multimedia-Erlebnis zu bieten.
- Optimierte Methode zur Listensymbol-Akquisition: Die Methode zur Akquisition von Listensymbolen wurde verbessert, was zu einer schnelleren und zuverlässigeren Symbol-Ladezeit führt.

### Behoben
- Problem mit der falschen Anzeige des Aktivierungsstatus in mehreren Fenstern beheben: Ein Problem wurde behoben, bei dem der Aktivierungsstatus bei geöffneten mehreren Fenstern falsch angezeigt wurde.

---

## [1.0.0] - 2024-06-29

### Hinzugefügt
- Umschalten zwischen hellem und dunklem Modus: Wählen Sie zwischen hellem und dunklem Anzeigemodus, um Ihren Vorlieben zu entsprechen.
- Anpassbare Schriftgröße: Passen Sie die Schriftgröße an, um ein komfortableres Leseerlebnis zu bieten.
- Anpassbares Schnittstellenlayout: Personalisieren Sie das Schnittstellenlayout entsprechend Ihren Nutzungsgewohnheiten.
- Personalisierungsoptionen: Fügen Sie bunte Hintergründe und Hintergrundbilder hinzu, um Ihr Seitenpanel einzigartig zu machen.
- Erweiterte Tab-Verwaltung: Miniaturansichten, umfangreiche Sortier- und Anzeigeoptionen sowie ein umfassendes Aktionsmenü für eine effiziente Tab-Verwaltung.
- Suchfunktion: Suchen Sie schnell nach kürzlich geschlossenen Tabs oder durchsuchen Sie Ihren Verlauf, um das zu finden, was Sie benötigen.
- Bild-in-Bild-Modus: Wechseln Sie nahtlos in den Bild-in-Bild-Modus, wenn Sie Tabs wechseln oder durch Seiten scrollen.
- Automatische Gruppierung: Erstellen oder treten Sie automatisch Gruppen basierend auf derselben Domain bei, um eine bessere Organisation zu gewährleisten.
- Lesefortschrittsleiste: Verfolgen Sie Ihren Lesefortschritt in Echtzeit, um zu wissen, wie weit Sie gelesen haben.
- Wiedergabefortschrittsleiste: Steuern Sie die Multimedia-Wiedergabe mit Optionen zum schnellen Vor- und Zurückspulen, zur Lautstärkeregelung und zur Anpassung der Wiedergabegeschwindigkeit.
