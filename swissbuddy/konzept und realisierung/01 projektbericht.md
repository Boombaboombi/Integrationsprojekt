Titel der Arbeit
SwissBuddy – Kompakte Alltagshilfe für Thai‑Neuzuzügerinnen in der Schweiz

Lehrgang
Dipl. Wirtschaftsinformatiker HF – Integrationsprojekt (Feusi)

Art der Arbeit
Projektarbeit (Konzept und Realisierung)

Abgabedatum
29.10.2025

Verfasser
Hofer Frédéric

Dozierende
Frank Liebermann (Konzept) / Thomas Benz (Realisierung)

1 Einleitung und Ausgangslage
Ich habe mit SwissBuddy eine schlichte, schnell verständliche Web‑App entwickelt, die
Thai‑Neuzuzügerinnen in der Schweiz beim Ankommen unterstützt. In den ersten Wochen
entscheiden kleine Hürden über das Sicherheitsgefühl im Alltag: einfache Wörter, kurze
Dialoge, Orientierung im öffentlichen Verkehr sowie grundlegende Kostenfragen. In genau diesen
Situationen möchte SwissBuddy helfen – ohne Registrierung, ohne Werbung und ohne ablenkende
Komplexität. Der Prototyp läuft lokal im Browser und ist bewusst leichtgewichtig gehalten.

Aus persönlicher Motivation heraus – meine Verlobte kommt aus Thailand – habe ich in den
letzten Wochen erlebt, wie stark Sprache über Selbstständigkeit entscheidet. Darum habe ich
eine Lösung mit klarem Fokus umgesetzt: Vokabeln mit Aussprache, ein überschaubares Quiz
zum Festigen, kompakte ÖV‑Tipps und ein kleiner Währungsrechner für THB, CHF und EUR.
Die Benutzeroberfläche steht in Deutsch, Thai, Italienisch, Englisch und Französisch zur
Verfügung; zusätzlich gibt es einen Dark‑Mode.

2 Zielsetzung
Ziel des MVP war es, einen funktionsfähigen Prototypen zu liefern, der die wichtigsten
Anwendungsfälle abdeckt und in einer kurzen Sitzung demonstriert werden kann. Konkret:
– eine Landingpage als Einstieg,
– eine Vokabelliste mit 51 Begriffen in DE/FR/IT/EN, jeweils ins Thai übersetzt, mit Suche
und einem Play‑Button zur Aussprache,
– ein Vokabel‑Quiz mit frei wählbaren Längen (5/10/20/Alle 51),
– ÖV‑Tipps als kompakten Wissensanker,
– einen Währungsrechner mit Live‑Berechnung und schneller Umkehr der Währungspaare,
– vollständige UI‑Lokalisierung (DE/TH/IT/EN/FR) samt Dark‑Mode.

3 Vorgehen und Methodik
Ich habe in kurzen, klar geschnittenen Arbeitspaketen gearbeitet. Inhaltlich stand der
Nutzennachweis im Vordergrund: Was hilft der Zielgruppe wirklich in der ersten Woche in der
Schweiz? Aus diesem Grund sind alle Module bewusst knapp gehalten und sofort benutzbar.
Technisch ist der Prototyp eine schlanke Frontend‑App für den Browser. Die Aussprache erfolgt
über die Web‑Speech‑Synthesis‑Schnittstelle des Geräts. Der Währungsrechner bindet eine
öffentliche Currency‑API ein und rechnet Eingaben direkt beim Tippen um. Die Daten werden im
Frontend gehalten; ein Server ist für den MVP nicht erforderlich. Gehostet wird lokal.

4 Umsetzung (Realisierung)
Die Startseite führt übersichtlich zu den vier Bereichen. Das Vokabel‑Modul enthält 51 häufige
Alltagsbegriffe. Eine Suche reduziert die Liste dynamisch. Bei jedem Eintrag startet ein
Play‑Button die Aussprache. Das Quiz nutzt denselben Wortschatz. Die Anzahl Fragen ist
wählbar; Antworten werden sofort visuell bewertet. Am Ende erhält die Nutzerin eine klare
Rückmeldung („Du hast X von Y richtig“) und kann direkt neu starten. Der Währungsrechner
unterstützt THB, CHF und EUR. Ein Tausch‑Button wechselt die Richtung der Umrechnung, das
Resultat aktualisiert sich live. Die ÖV‑Tipps geben in kurz gefasster Form Orientierung für Zug
und Bus. Die gesamte Oberfläche ist in fünf Sprachen verfügbar; der Dark‑Mode ist jederzeit
umschaltbar.

5 Abgrenzung und weiterer Ausbau
Im MVP sind Inhalte und Funktionen auf das Wesentliche reduziert. Für eine zweite Phase plane
ich: ausformulierte ÖV‑Guides mit Beispielen und Screens, hochwertige Audio‑Clips statt der
geräteabhängigen TTS‑Stimme, Favoriten/Lesezeichen, Lernfortschritt, sowie das Hosting unter
swissbuddy.ch mit HTTPS und einfacher Telemetrie.

6 Risiken und Hürden
Die grösste Hürde war die private Zeitknappheit aufgrund medizinischer Themen in der Familie.
Zudem verliert KI‑Unterstützung bei mehreren Iterationen häufig den Gesamtzusammenhang,
weshalb ich kleine Arbeitspakete und saubere Zwischenergebnisse bevorzugt habe. Inhaltlich war
das Sprachkonzept anspruchsvoll: Die UI‑Sprache und die zu lernende Sprache sind nicht identisch,
was in der Struktur sauber getrennt sein muss. Technisch liefert die TTS‑Schnittstelle je nach
Gerät eine sehr unterschiedliche Qualität; insbesondere auf iOS wirkt die Stimme metallisch.

7 Testkonzept (Auszug)
Ich habe die Kernfälle manuell geprüft: Wechsel der UI‑Sprache, Suche in der Vokabelliste,
Aussprache‑Buttons, Quiz‑Modi inklusive korrektem Scoring und Markierung der richtigen
Lösung, Sichtbarkeit der ÖV‑Tipps, Live‑Berechnung und Swap im Währungsrechner sowie das
Theme‑Toggling. Zusätzlich habe ich einen Offline‑Fall für den Währungsrechner betrachtet:
ohne Netz erscheint kein Ergebnis, die App bleibt stabil.

8 Schlussbetrachtung
Der MVP erfüllt seinen Zweck: Er zeigt, dass eine sehr schlanke Web‑App mit klarer
Zielgruppenfokussierung echten Nutzen stiften kann, direkt ab dem ersten Tag in der Schweiz.
In der nächsten Phase werde ich die Inhalte vertiefen, echte Audio‑Aufnahmen produzieren und
die App unter swissbuddy.ch verfügbar machen.
