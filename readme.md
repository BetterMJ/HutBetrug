# HutBetrug - Gruppe Cookie
## Aufgabenstellung
Dieses Projekt haben wir als Schularbeit in einer 4er Gruppe gemacht. Das Programm soll den Benutzer raten lassen, unter welcher der 3 Hüte die Münze, also der Coin, ist. Hier, bei diesem Portfolio, gehe ich mehr zu einem spezifischen Vorgang, wie man mehrere Form-Applikationen öffnet und wie man diese wieder versteckt.

1. Der Leser lernt, was eine Form-Applikation ist.
2. Der Leser erfährt, wie man eine neue Form-Applikation erstellt.
3. Der Leser lernt, wie man mehrere Form-Applikaitonen gleichzeitig öffnet.
4. Der Leser erfährt, wie man eine Form-Applikation schliesst, wenn man eine andere öffnet.

## Inhalt
### Inhalt
Unter einer Form-Applikation kann man sich ein Fenster vorstellen, welches komplett leer ist, jedoch kann man auf diesem auch Funktionen einfügen, wie zum Beispiel einen Knopf, Bilder und mehr. Dadurch kann man einfache oder komplexere Programme erstellen, wie unseres in diesem Fall.

Es ist gar nicht so schwer, wie man denkt, ein neues Fenster zu machen. Zuerst geht man zum Projekt, drückt Rechts-Klick darauf und wählt "Hinzufügen" aus, danach fügt man ein "Windows Forms Application" hinzu. Jetzt haben wir bereits ein weiteres Fenster hinzugefügt und können Änderungen anwenden.
Um mehrere Fenster öffnen zu können, fängt es mit dem Code an; gehe zum Haupt-Code und schreibe folgendes in zum Beispiel einen Button:

`Form2 settingsForm = new Form2();`

`settingsForm.Show();`

Nun haben wir 2 Form-Applikationen offen.
Jetzt muss man nur noch schauen, dass man das mainForm, das Form welches man zu Beginn hatte, noch schliesst, damit sich nur das neue Fenster zeigen lässt. Um die neue Form-Applikation zu schliessen, können wir es einfach mit `mainForm.Hide();` bei dem Start des Programms, unter `InitializeComponent();`, welches Sie bereits im Code haben, einfügen. Dieses muss man in den Code von der neuen Form-Applikation einschreiben.

Nun sind wir schon fast fertig, jetzt wollen wir nur noch, dass man das Haupt-Form, also das mainForm wieder öffnet, wenn man das neue Fenster schliesst.
Um dieses durchzuführen müssen wir einfach einen kurzen Code schreiben:

```private void settingsForm_FormClosed(object sender, FormClosedEventArgs e)```

        {
            mainForm.Show();
        }
   
Nun haben wir erfolgreich eine neue Form-Applikation aufgemacht, wieder zugemacht, während das mainForm geschlossen war.

### Bilder
Hier eine Bilddarstellung, wie es für den Benutzer aussehen könnte, wenn man ein neues Fenster öffnet und schliesst:
![Programm](https://i.imgur.com/hmW6t4J.jpg)

Beim unteren Bild ist nur 1 Fenster offen:

![Programm](https://i.imgur.com/R16NKES.jpg)
![Programm](https://i.imgur.com/pPxgKDO.jpg)

### Video
Hier ein kurzes Video zu allen Form-Applikationen und deren Funktionen bei unserem Programm:
[![](https://i.imgur.com/UdsPUGR.jpg)](https://youtu.be/hF-tRYMbz3U)

## Reflexion / Verifikation
Ich fand es sehr spannend, dass wir in einer 4er Gruppe mit Leuten arbeiten durften, welche wir noch nicht kannten. Nach gewisser Zeit haben wir uns sehr gut verstanden, haben sehr effizient gearbeitet und unsere Stärken ausgenutzt, dadurch kamen wir sehr schnell voran. Zu Beginn hatten wir mühe uns zu verstehen und die Stärken zu finden, jedoch kam dieses mit der Zeit. Nächstes Mal ist es sicher eine gute Idee mit einem Kennenlernspiel zu starten, damit man sich sehr schnell versteht und die Stärken einschätzen kann.

Mein Banknachbar Ruzicic weiss nun was eine Form-Applikation ist und kann eines erstellen, er erfuhr auch wie man mehrere Form-Applikationen öffnet. Er weiss jedoch auch, wie man nur 1 Fenster offen haben kann.
