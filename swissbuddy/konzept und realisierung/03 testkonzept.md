Testkonzept und Testfälle (MVP)

Ziele
— Kernfunktionen sind ohne Fehlermeldungen nutzbar.
— Lokalisierung der Oberfläche in DE/TH/IT/EN/FR funktioniert konsistent.
— TTS gibt eine hörbare Ausgabe; das Quiz wertet korrekt; der Währungsrechner rechnet live.

Umgebung
Aktuelle Desktop‑Browser (Chrome, Edge, Firefox). Optional iOS Safari für TTS‑Eindruck.
Internetverbindung für die Currency‑API.

Ausgewählte Testfälle
T1 UI‑Sprache wechseln: Startseite, Sprache auf TH/IT/EN/FR stellen; alle Labels passen sich an.
T2 Suche: Vokabeln, Suchbegriff „Ticket“, Liste filtert korrekt.
T3 Aussprache: Vokabel „Hallo“, Play‑Button erzeugt TTS‑Ausgabe.
T4 Quiz‑Längen: 5/10/20/Alle spielen; am Ende korrekte Anzeige „X von Y“.
T5 Richtig/Falsch‑Markierung: falsche Auswahl zeigt rot, richtige Lösung wird grün markiert.
T6 ÖV‑Tipps: Seite lädt, Inhalte sind sichtbar.
T7 Live‑Berechnung: Betrag tippen; Ergebnis aktualisiert sich bei Eingabe; Swap wechselt Paare.
T8 Dark‑Mode: Schalter toggelt konsistent.
T9 Offline‑Fall: Netz trennen; Währungsrechner öffnen; keine Abstürze.