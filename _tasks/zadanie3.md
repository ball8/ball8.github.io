---
layout: task
title: Zadanie 3
description: XML prezentácia
weight: 3
---

+ Vytvoril som si DTD, ktoré definuje elementy prezentácie.
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

