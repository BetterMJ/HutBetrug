# HutBetrug - Gruppe Cookie
## Aufgabenstellung
Dieses Projekt haben wir als Schularbeit in einer 4er Gruppe gemacht. Das Programm soll den Benutzer raten lassen, unter welcher der 3 Hüte die Münze, also der Coin, ist. Hier, bei diesem Portfolio, gehe ich mehr zu einem Spezifischen Vorgang, wie man mehrere Forms öffnet und wie man diese wirder versteckt.

1. Der Leser lernt, was ein "Form" ist.
2. Der Leser erfährt, wie man ein neues Form erstellt.
3. Der Leser lernt, wie man mehrere Forms gleichzeitig öffnet.
4. Der Leser erfährt, wie man ein Form schliesst, wenn man ein anderes offen hat.

## Inhalt
### Inhalt
Unter einem Form kann man sich ein Fenster vorstellen, welches komplett leer ist, jedoch kann man auf diesem auch Funktionen einfügen, wie zum Beispiel einen Knopf, Bilder und mehr. Dadurch kann man einfache oder komplexere Programme erstellen, wie unseres in diesem Fall.

Es ist gar nicht so schwer, wie man denkt, ein neues Form zu machen. Zuerst geht man zum Projekt, drückt Rechts-Klick darauf und wählt "Hinzufügen" aus, danach fügt man ein "Windows Form" hinzu. jetzt haben wir bereits ein weiteres Form hinzugefügt und können Änderungen anwenden.
Um mehrere Forms öffnen zu können, fängt es mit dem Code an; gehe zum Haupt-Code und schreibe folgendes:

`Form2 settingsForm = new Form2();`
`settingsForm.Show();`

Nun haben wir 2 Forms offen.
Jetzt muss man nur noch schauen, dass man das mainForm, das Form welches man zu Beginn hatte, noch schliesst, damit sich nur das neue Fenster zeigen lässt. Um das neue Form zu schliessen, können wir es einfach mit `mainForm.Hide();` bei dem Start des Programms, unter `InitializeComponent();`, welches Sie bereits im Code haben, einfügen. Dieses muss man in den Code von dem neuen Form einschreiben.

Nun sind wir schon fast fertig, jetzt wollen wir nur noch, dass man das Haupt-Form, also das mainForm wieder öffnet, wenn man das neue Fenster schliesst.
Um dieses durchzuführen müssen wir einfach einen kurzen Code schreiben:

```private void settingsForm_FormClosed(object sender, FormClosedEventArgs e)```

        {
            mainForm.Show();
        }
   
Nun haben wir erfolgreich ein neues Form aufgemacht, wieder zugemacht, während das mainForm geschlossen war.

### Bilder
Hier noch ein kurzer Schritt bei Schritt Bilddarstellung, wie es für den Benutzer aussehen könnte, wenn man ein neues Fenster öffnet uns schliesst:
![Programm](https://i.imgur.com/hmW6t4J.jpg)
![Programm](https://i.imgur.com/R16NKES.jpg)
![Programm](https://i.imgur.com/pPxgKDO.jpg)

### Video
Hier ein kurzes Video mit allen Forms und deren Funktionen:
[![](https://i.imgur.com/UdsPUGR.jpg)](https://youtu.be/hF-tRYMbz3U)

## Reflexion / Verifikation
Gut
Schlecht
Nächstes Mal

Mein Banknachbar Ruzicic kann bestätigen, dass 
