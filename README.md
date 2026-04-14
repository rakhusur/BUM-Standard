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