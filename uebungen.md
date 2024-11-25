![Comquent Academy](./images/comquent-academy-logo.png?raw=true "Comquent Academy")
# GitHub Copilot Workshop - Übungen
### Übung 1 - Gute Prompts erstellen
#### In dieser Übung lernen wir, wie Copilot anhand der von uns bereitgestellten Informationen Code generiert.
1. Erstelle eine neue Datei. Wir nutzen für dieses Beispiel eine JavaScript-Datei. Erstelle sie über das Interface oder gib Folgendes in deinem Terminal ein:

  ```bash 
  code index.js
  ```

   Anschließend sollte die Datei in deinem Editor geöffnet sein.

2. Sehen wir uns nun an, wie Copilot auf eine sehr generische Anfrage reagiert. Wir kommunizieren dabei über Kommentare. Gib in deiner `index.js` folgenden Kommentar ein:

  ```javascript
  // function to parse data
  ```

3. Wenn du jetzt Enter drückst, sollte Copilot direkt Code für die nächste Zeile vorschlagen. Durch Drücken von "Tab" kannst du diese Zeile akzeptieren, woraufhin direkt der nächste Vorschlag erscheint. Falls nicht, drücke zunächst erneut "Enter", um in die nächste Zeile zu springen. So kannst du weitermachen, bis die Funktion vollständig ist.
  
4. In manchen Fällen kann es vorkommen, dass auch nach mehreren Sekunden kein Vorschlag angezeigt wird. Dann kann Copilot durch Eingeben des ersten zu erwartenden Buchstabens (in unserem Fall ein "f" für "function") ein kleiner "Schubser" gegeben werden, und der Vorschlag für den nächsten Teil des Codes sollte erscheinen.
    
Ein ähnliches Problem kann sich übrigens ergeben, wenn wir die Anfrage auf Deutsch formulieren:

  ```javascript 
  // Funktion zum Parsen von Daten
  ```

Hier ist es noch ein wenig wahrscheinlicher, dass Copilot nicht auf Anhieb einen sinnvollen Vorschlag macht, sondern möglicherweise sogar selbst einen weiteren Kommentar hinzufügen möchte. Auch hier hilft das "Anstupsen" durch Eingabe des ersten Buchstabens, den wir sehen wollen: "f".

5. Unser Prompt per Kommentar ist in jedem Fall noch nicht spezifisch genug, damit Copilot weiß, was wir tun möchten. Entferne den Code und versuche es mit:
  ```javascript
  // function to parse url
  ```

6. Drücke "Enter" und du wirst vermutlich eine Zeile wie diese sehen:
  ```javascript
  function parseURL(url) {
  ```
7. Drücke "Tab", um den Vorschlag anzunehmen, und wieder "Enter". So kannst du dir Stück für Stück deine Funktion "zusammenbauen" lassen. Wie zuvor gilt: Sollte kein (brauchbarer) Vorschlag kommen, hilft das "Anstupsen" durch Eingabe eines Buchstabens (oft auch schon durch Tasten wie Leertaste, Backspace oder Enter).  

8. Wirklich zufrieden wirst du mit dem Ergebnis wohl nicht sein. Copilot kann auch alternative Vorschläge anzeigen. Lösche dazu alles bis auf die erste Zeile der Funktion und platziere den Cursor am Ende der Zeile.

9. Drücke "Strg" + "Enter". Es öffnet sich ein Fenster mit weiteren Vorschlägen. Unter Umständen kann das Generieren dieser Vorschläge ein paar Sekunden dauern. Diese werden in ihrer Vollständigkeit und Qualität mitunter stark variieren. Gefällt dir einer, klicke auf "Accept suggestion", um den Code zu übernehmen.

10. Lass uns jetzt noch einmal versuchen, eine noch spezifischere Anfrage zu stellen. Lösche deinen gesamten Code, und gib anstelle eines Kommentars einen Funktionsnamen ein. Drücke noch nicht "Enter" oder "Tab":
  ```javascript
  function splitURLandReturnComponents
  ```
11. Mit diesem Namen sollte Copilot eine vollständige Funktion vorschlagen - tatsächlich sogar mehrere. Bewege die Maus über den Code und ein kleines Fenster sollte erscheinen. Hier siehst du, wie viele Optionen zur Auswahl stehen. Klicke auf ">" bzw. "<", um die Optionen durchzuschalten, und auf "Akzeptieren" ("Tab"), um den jeweiligen Vorschlag in deinen Code zu übernehmen.