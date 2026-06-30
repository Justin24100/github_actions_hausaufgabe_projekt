# Abgabe: GitHub Actions mit Bash Skripten

## Repository Link

https://github.com/Justin24100/github_actions_hausaufgabe_projekt

---

## Nachweise der Ausführung

### Aufgabe 1: Manuelle Namensbegrüßung

Die Pipeline wurde erfolgreich manuell gestartet.


---

### Aufgabe 2: Manuelle Projektprüfung mit Selectfeld

Die Pipeline wurde erfolgreich manuell gestartet.



---

### Aufgabe 3: Automatische Pipeline bei Push auf main

Die Pipeline wurde erfolgreich durch einen Push auf den Branch main gestartet.



---

# Aufgabe 1: Manuelle Namensbegrüßung

Die Pipeline `01 Manuelle Begruessung` wurde manuell über den Button `Run workflow` gestartet.  
Beim Start konnte ein Name eingegeben werden. Dieser Name wurde in der YAML-Datei als Input `student_name` verwendet. Danach wurde der Wert als Umgebungsvariable `STUDENT_NAME` an das Bash-Skript `scripts/01_manual_greeting.sh` übergeben.

Eingegebener Name: Justin

Das Bash-Skript hat anschließend eine Begrüßung mit dem eingegebenen Namen ausgegeben.  
Die Pipeline wurde erfolgreich ausgeführt.

---

# Aufgabe 2: Manuelle Projektprüfung mit Selectfeld

Die Pipeline `02 Manuelle Projektpruefung` wurde ebenfalls manuell über den Button `Run workflow` gestartet.  
Beim Start wurden Werte für `check_type`, `target_env` und `show_details` ausgewählt. Diese Werte wurden in der YAML-Datei als Inputs verwendet und als Umgebungsvariablen an die Bash-Skripte übergeben.

Ausgewählte Werte:

```text
check_type: full
target_env: dev
show_details: true