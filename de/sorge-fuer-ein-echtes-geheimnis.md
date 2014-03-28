Sorge für einen individuellen Sicherheitsschlüssel (secret)
sicherheit
Stelle sicher, dass Dein Produktivsystem einen individuellen Sicherheitsschlüssel verwendet. Prüfe dies in der Datei `app/config/parameters.yml`:

    secret:  please_use_a_real_secret_here

Der Standardschlüssel ist *nicht* wirklich geheim und muss *unbedingt* durch einen zufälligen ersetzt werden.
