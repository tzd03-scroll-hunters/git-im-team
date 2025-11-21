# Setup für ein (Final) Fullstack Project

## GitHub Orga erstellen

Auf Github oben rechts das + Symbol klicken => New organisation. Konstenlosen Plan wählen. Team Member inviten. Fertig!

## Ein Repo für Frontend und Backend oder lieber 2? 

Lieber zwei getrennte => weniger Quellen für versehentliche Merge-Konflikte. Und etwas einfacher zu deployen


## Ordner-Struktur der Repos

Nur EINE Person setzt Repo und Ordner-Struktur auf (aber am besten zusammen im Team alle drüberschauen). 

Ordner sollten später, wenn es geht, niemals mehr UMBENANNT, VERSCHOBEN oder GELÖSCHT werden 
=> diese Art Changes produzieren die kompliziertesten Merge-Konflikte.

Neue (Unter-) Ordner später hinzufügen ist kein Problem!


## Das Repo zur GitHub Orga bringen?

Einfachster Weg: Repo lokal erstellen und die Ordner-Struktur erstellen. Danach direkt aus VsCode zu GitHub hochladen. Es landet nun im eigenen Account

Danach: Zu Repo > Tab "Settings" => ganz nach unten scrollen zu "Danger Zone" => Transfer => und dann die Orga angeben


## Git im Team Prozess (kurz)

(wenn ihr "dev" als default Branch benutzt => ersetze in dieser Anleitung überall "main" durch "dev")

- Sicherstellen dass ich zum Start auf main (dev) Branch bin: `git checkout main`
- Auf letzten Stand von Main upgraden: `git pull`
- Branch erstellen: `git checkout -b features/<meinFeature>` meinFeature ersetzen durch dein Feature
- Coden coden coden
- Fertig mit Coden => `git add .` und `git commit`
- Checken, ob in der Zwischenzeit Leute was im Main geändert haben: `git pull origin main`
- Wenn es Merge Konflikte gibt: In unserem Branch fixen oder in Team-Meeting (wenn unklar, wie wir das lösen)
- Wenn es keine Konflikte gibt / alle behoben sind: PULL REQUEST auf Github stellen (=> grüner Button "OPEN & COMPARE PullRequest")
- Wenn die Meldung kommt "Able to Merge" => branch einmergen
- Danach: Den main branch lokal aktualisieren: `git checkout main` und danach `git pull`
- Danach: NÄCHSTEN Features branch erstellen git checkout -b /featues/naechstesFeature
- Und dann wiederholt sich alles immer wieder :)


