---
layout: default
title: Failu lasīšana/raksīšana
description: ~
grand_parent: Programmēšana
parent: Python
nav_order: 8
---
# Failu - lasīšana, rakstīšana

Python programmēšanas valoda ļauj nolasīt failus un to saturu.

~~~python
with open('data.txt', 'r') as f:
    dati= f.read()
~~~

Kur data.txt ir faila nosaukums (jāatrodas tajā pašā mapē, kur atrodas `.py` fails), `r` parametrs norāda, ka fails tiek lasīts - read. Savukārt, mainīgais `dati` saturēs vārdnīcu ar rindām no faila. 

Ierakstīt failā:

~~~python
with open('data.txt', 'w') as f:
    dati= 'Šo tekstu ierakstīt failā'
    f.write(dati)
~~~

Šajā gadījumā tiek ierakstīts failā teksts - pārrakstot faila saturu. 

Ierakstīt failā:

~~~python
with open('data.txt', 'a') as f:
    dati= 'Šo tekstu ierakstīt failā'
    f.write(dati)
~~~