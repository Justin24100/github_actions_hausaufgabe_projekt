# Abgabe: GitHub Actions mit Bash Skripten

## Repository Link

Link: TODO

## Nachweise

- Aufgabe 1: TODO Screenshot oder kurzer Nachweis einfuegen
- Aufgabe 2: TODO Screenshot oder kurzer Nachweis einfuegen
- Aufgabe 3: TODO Screenshot oder kurzer Nachweis einfuegen

## Aufgabe 1: Manuelle Namensbegruessung

Diese Pipeline wird manuell ueber den Button `Run workflow` gestartet. Beim Start kann im Feld `student_name` ein Name eingegeben werden. Dieser Wert wird in der YAML Datei als Umgebungsvariable `STUDENT_NAME` an das Skript `scripts/01_manual_greeting.sh` uebergeben. Das Skript gibt eine Begruessung aus und zeigt, dass es durch eine manuelle Pipeline gestartet wurde.

Eingegebener Name: TODO

Ausgabe: TODO

## Aufgabe 2: Manuelle Projektpruefung mit Selectfeld

Diese Pipeline wird ebenfalls manuell ueber `Run workflow` gestartet. Beim Start werden `check_type`, `target_env` und `show_details` ausgewaehlt. Die Umgebung und die Detailausgabe werden an `scripts/02_environment_info.sh` uebergeben, danach wird `scripts/03_project_check.sh` mit der Pruefart gestartet. Bei `quick` wird nur grundlegend geprueft, ob wichtige Projektbestandteile vorhanden sind; bei `full` werden zusaetzliche Informationen wie die Anzahl der Shell Skripte und der Inhalt des Log-Ordners ausgegeben.

Ausgewaehlte Werte: TODO

Was passiert bei `show_details=true`: Es werden zusaetzlich das Runner-Betriebssystem und der Arbeitsordner ausgegeben.

## Aufgabe 3: Automatische Pipeline bei Push auf main

Diese Pipeline startet automatisch, sobald ein Push auf den Branch `main` erfolgt. Deshalb ist hier kein `Run workflow` Button notwendig, weil der Trigger nicht manuell, sondern durch den Push ausgeloest wird. Zuerst wird das Skript `scripts/04_main_pipeline.sh` ausgefuehrt. Danach startet der einfache Test `tests/simple_test.sh`.

Ausgefuehrte Skripte:

- `scripts/04_main_pipeline.sh`
- `tests/simple_test.sh`

## Kontrollliste

- [ ] Projekt liegt in einem GitHub Repository
- [ ] Drei YAML Dateien liegen unter `.github/workflows`
- [ ] Aufgabe 1 wurde manuell gestartet und ist erfolgreich gelaufen
- [ ] Aufgabe 2 wurde manuell gestartet und ist erfolgreich gelaufen
- [ ] Aufgabe 3 wurde durch Push auf `main` gestartet und ist erfolgreich gelaufen
- [ ] Repository Link wurde eingetragen
- [ ] Screenshots oder kurze Nachweise wurden eingefuegt
