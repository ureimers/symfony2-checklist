Installiere einen PHP-Beschleuniger
leistung
Symfony2 ist ein flexibles und mächtiges Framework, was sich auf die Ausführungsgeschwindigkeit auswirkt. Zwar ist die prod-Umgebung deutlisch schneller als die gewöhnliche dev-Umgebung, doch das reicht nicht.

Um die Anwendung im Live-Betrieb ordentlich anzukurbeln ist es _sehr_ empfohlen, einen PHP-Beschleuniger wie APC zu installieren.

### Auf einem dedizierten Server

#### Linux
Um APC auf einer Debian-ähnlichem Linux-Distribution zu installieren, führe folgendes aus:

    apt-get install php-apc

Je nach Distribution ist der Kommando / der Package-Manager anzupassen.

#### Windows
Hebe die Kommentierung der folgenden Zeile aus Deiner `php.ini` auf:

    extension=php_apc.dll

#### In jedem Fall
Nach der Installation muss die PHP-Erweiterung aktiviert werden. Dies geschieht durch das Anfügen der folgenden Zeilen  ans Ende Deiner `php.ini` (wenn nicht bereits vorhanden aber auskommentiert):

    [APC]
    apc.enabled=1

### Auf einem shared Host
Auf einem shared Host ohne SSH-Zugriff solltest Du Dich mit Deinem Administrator in Verbindung setzen und ihn davon überzeugen, dass es besser für seine Server ist, einen PHP-Beschleuniger aktiviert zu haben.

* _Siehe [APC on the PHP doc](http://php.net/manual/en/book.apc.php)_
