---
layout: task
title: Zadanie 1
description: Osobná webová prezentácia na GitHub pages
weight: 1
---

Na stránke využívam 5 layout-ov :
+ profil.html - na stránke myprofil.html (profil)
+ layout1.html - na stránkach wpub.html (Webové publikovanie), freetime.html (Voľnočasové aktivity)
+ task.html - na stránkach jednotlivých zadaní
+ poem.html - na stránkach jednotlivých básničiek
+ default.html - na stránkach index.html (Domov) a project.html (Moje projekty)

V rámci šablón som podľa požiadaviek použil tieto elementy :
+ **premenné** - napríklad v layout-e profil.html : title, myname, job, age, email
+ **kolekcie** -
1. v layout-e task.html : tasks
2. na stránke wpub.html : poems
+ **tagy a filtre** -
1. include : vo všetkých layout-och (vkladal som navigation bar)
2. for : v layoute task.html (vkladal som odkazy na ostatné zadania, aby sa pri prezeraní jendého zadania dalo otvoriť hned aj druhé zadanie bez toho, aby sa človek musel vrátiť na stránku zadaní)
3. assign : v layout-e task.html
4. if : v layout-e task.html
5. append : v layoute task.html
6. upcase : v layoute profil.html
+ **plugin** : *reading_time* zo stránky jekyll.tips, ktorý som upravil, aby zobrazoval slovenský text a nie anglický, používam ho v layout-e
poem.html, nad každou básničkou zobrazí informáciu, koľko minút bude čitateľovi približne trvať, kým ju prečíta.
