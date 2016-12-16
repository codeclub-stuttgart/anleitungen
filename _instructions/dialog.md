---
layout: instruction
title: "Mit Figuren reden"
---

<br>
<br>
<br>

![](dialog/hello-cat.png)

<div class="page-break"></div>

## Figur sprechen lassen

Dieser Block zeigt eine Sprechblase 2 Sekunden lang an, erst danach wird der Block darunter gestartet

```blocks
    sage [Hallo!] für (2) Sek.
```

Dieser Block zeigt eine Sprechblase und macht keine Pause  

```blocks
    sage [Hallo!]
```

Du musst die Sprechblase mit einem zweiten leeren Block wieder verstecken

```blocks
    sage []
```

<div class="checklist-symbol">Checkliste</div>

- Probiere einmal beide Blöcke aus
- Schau einmal was die <span class="visual-block">denke</span>-Blöcke machen     

<div class="test-symbol">Teste dein Projekt</div>

<div class="page-break"></div>

## Mit Figur reden

Deine Figuren können auch Fragen stellen

<div class="checklist-symbol">Checklist</div>

- Wähle eine Figur aus

- Füge folgende Blöcke hinzu

```blocks
    Wenn die grüne Flagge angeklickt
    frage [Soll ich die Schatztruhe öffnen?] und warte
```

<div class="test-symbol">Teste dein Projekt</div>

Es wird jetzt ein Textfeld angezeigt. Der Computer merkt sich dann was du hineinschreibst. 

![](dialog/answer-input.png)

Um mit der Antwort etwas zu machen brauchen wir im nächsten Schritt den <span class="sensor-value">Antwort</span>-Block 

- Füge unter dem <span class="sensor-block">frage</span>-Block diese Blöcke ein 

```blocks
    falls <(Antwort) = [ja]> dann
        sage [Toll, ganz viel Gold] für (2) Sek.
    sonst
        sage [Dann eben nicht] für (2) Sek. 
    Ende
```

<div class="test-symbol">Teste dein Projekt</div>

<div class="page-break"></div>

-  Du kannst auch zwischen mehreren Antworten unterscheiden. 
   
   Füge noch einen weiteren <span class="control-block">falls</span>-Block ein  


```blocks
    falls <(Antwort) = [ja]> dann
        sage [Toll, ganz viel Gold] für (2) Sek.
    sonst
        falls <(Antwort) = [nein]> dann
            sage [Dann eben nicht] für (2) Sek.
        sonst
            sage [Ich weiß nicht was du meinst] für (2) Sek.
    Ende
```

<div class="test-symbol">Teste dein Projekt</div>
