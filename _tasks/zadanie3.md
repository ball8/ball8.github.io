---
layout: task
title: Zadanie 3
description: XML prezentácia
weight: 3
---

+ Vytvoril som si DTD, ktoré definuje elementy a štruktúru prezentácie.
+ Vytvoril ukážkovú preznetáciu o ovocí pomocou xml.
+ Vytvoril som XSLT pre konverziu zo xml do xhtml + parametrizácia (zobrazovanie čísel slajdov).
+ Vytvoril som si vlastný CSS súbor.
+ -Transformáciu do PDF som nevytvoril kvôli nedostatku času.

V XSLT som využil rôzne elementy, uvádzam zoznam:
+ apply-templates - aplikovanie šablón
+ for-each - iterovanie cez elementy
+ if - podmienka (if test="expression")
+ number - na číslovanie slajdov
+ template - vytvorenie šablón
+ value-of - pre získanie hodnoty elementu
+ attribute - vytvorenie atribútu pre element
+ choose - kvôli použitiu when, ktoré bez tohto nejde použiť
+ when - na zisťovanie, má obrázok atribút width a height

Keďže DTD neumožňuje definovať štruktúru podľa hodnoty atribútu a typy slajdov som riešil cez atribút **type**,
každý slide môže mať všetky elementy, ako textblock (text, list, numberedlist), image. Konkrétnejšie slide má dieťa content
heading* ,textblock* ,image*, footer. Vyriešil som to, že pre každý typ slajdu mám šablónu a každá spracuje len niektoré elementy,
aj keď podľa DTD ich tam používateľ môže dať, v prezentácií sa nezobrazia.

Typy slideov:
+ front - úvodný slajd
+ content - slajd s automaticky generovaným obsahom prezentácie
+ normal - obyčajný generický slajd, šablóny na ňom spracujú všetky elementy
+ figure - šablóny spracujú len obrázok
+ final - záverečný slajd graficky odlíšený od ostatných
