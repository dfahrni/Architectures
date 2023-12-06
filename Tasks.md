# Übung Architekturen

Entwickle und implementiere eine Architektur für eine Chat-Applikation.

Halte dein Vorgehen, Überlegungen und Erkenntnisse in einem Dokument fest.
Schicke dieses am Ende der Unterrichtseinheit dem Dozenten.

Organisiert euch selbstständig in der Klasse, wie ihr die Aufgabe Lösen wollt.
Stellt sicher, dass alle verstehen, was gemacht wurde.

## Lernziele

Die Studierenden kennen verschiedene Architekturstile und deren Anwendung.
Die Studierenden könne die technischen Vorzüge spezifischer Entwicklungen im Bereich verteilter Computersysteme
analysieren und nachvollziehbar begründen. Sie können Sachverhalte klar erklären, um die Qualität des Feedbacks zu
optimieren.

## Aufgabenstellung

### Architektur

Die Applikation soll Chats zwischen einzelnen Usern sowie in Gruppen ermöglichen.
Alle Nachrichten sollen in einer Datenbank persistiert werden.

Dazu bietet sich die Publish-Subscribe in Kombination mit einer "Ports & Adaptors" Architektur an.

Entwirf eine Publish-Subscribe Architektur für diese Applikation!

Bestimme ebenfalls das Format der ausgetauschten Nachrichten.

Erstelle dazu ein Dokument in [Markdown](https://www.markdownguide.org/) mit [Mermaid](https://mermaid.js.org/).

### Implementierung

Nutze für die Implementierung dazu den Message-Broker "RabbitMQ" von [CloudAMQP](https://www.cloudamqp.com/).

Erstelle auf CloudAmPQ einen neuen Cluster und verbinde den einfachen [Beispielclient](client.html).

Erweitere die Beispielapplikation:

- Anzeige der verfügbaren User
- Erstellen von Gruppenchats