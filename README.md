# AAAB Formulare

Online-Formulare der AAAB GmbH. Jedes Formular hat einen eigenen Ordner.
Auf aaab.ch werden sie über WordPress-Seiten eingebunden.

| Formular | Ordner | Datei | Seite auf aaab.ch |
|---|---|---|---|
| Personalstammblatt | `/` (Hauptordner) | `formular.html` | aaab.ch/personalstammblatt |
| Bewertungsbogen Probetag | `/probetag/` | `feedback.html` | aaab.ch/probetag |
| Ferienantrag 2027 | `/ferienantrag/` | `index.html` | aaab.ch/ferienantrag |

Jeder Ordner hat eine kleine `index.html`, die auf das Formular weiterleitet
und die Vorschau für WhatsApp liefert. Links mit Angaben (`?vorname=...`)
werden dabei mitgegeben.

Ferienantrag: Mitarbeitende senden den Antrag (Supabase-Tabelle `ferienantraege`, art = antrag)
und schicken den Link an ihre Vorgesetzte. Der Link enthält den Antrag (`?a=`). Die Vorgesetzte
entscheidet (art = entscheid), dann geht die E-Mail an mitarbeiter@aaab.ch.
