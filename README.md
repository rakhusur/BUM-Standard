[![PDF](https://img.shields.io/badge/PDF-download-blue)](http://rakhusur.github.io/BUM-Standard/BUM-Standard.pdf)

# BUM-Standard

## Setup

Verwendet Tectonic für automatische Latex-Builds.

👉 Installation: <https://tectonic-typesetting.github.io/>

## Kompilieren

```bash
tectonic -X build
```

## Github-Actions

Bei jedem Push wird das Dokument automatisch kompiliert.
Wenn das auf dem main-branch passiert, wird das PDF auf Github pages hochgeladen und ist
über den Download-Button oben verfügbar.
Bei einem Version-Tag wird es außerdem dem [Release](https://github.com/rakhusur/BUM-Standard/releases) hinzugefügt.

## Latex-Commands
Hier ein Überblick über die wichtigsten Custom-Latex-Commands:

**\s \h \d \c** für Piks, Coeur, Karo und Treff. Im Fließtext sorgt bspw. \s{} dafür, dass nach dem Pik-Symbol ein Leerzeichen gesetzt wird.

**\begin{bids} \end{bids}** legt eine Tabelle mit zwei Spalten an, von der die rechte so breit ist wie nötig - Ideal für Erklärungen von Geboten ;)

Beispiel:<br>
\begin{bids}<br>
1\c & 12 Punkte, etc. \\\\ <br>
1\d & 12 Punkte, bla bla \\\\<br>
\end{bids}

Für Biettabellen innerhalb von Biettabellen, beispielsweise für Rebids, gibt es **\begin{subbids}**. Das sollte immer innerhalb der rechten Erklärungsspalte stehen, nicht in der linken Gebotsspalte.

Für offene Todos: \tbd{...}. Im Dokument steht dann TBD: ... und der Text ist rot.
