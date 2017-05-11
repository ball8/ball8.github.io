---
layout: task
title: Zadanie 3
description: XML prezentácia
weight: 3
---

+Vytvoril som si DTD, ktoré definuje elementy prezentácie.

**Tu vidno obsah DTD:**
<!ELEMENT presentation (author+,title,slide+)>
<!ELEMENT title (#PCDATA)>
<!ELEMENT author (#PCDATA)>
<!ELEMENT slide (content)>
<!ATTLIST slide type (front|content|normal|figure|final) "normal">
<!ELEMENT content (heading*,textblock*,image*, footer)>
<!ELEMENT footer (#PCDATA)>
<!ELEMENT heading (#PCDATA)>
<!ELEMENT textblock (text*, list*, numberedlist*)>
<!ELEMENT text (#PCDATA)>
<!ELEMENT numberedlist (listitem+)>
<!ELEMENT list (listitem+)>
<!ELEMENT listitem (#PCDATA)>
<!ELEMENT image (description*, width*, height*)>
<!ATTLIST image src CDATA #REQUIRED>
<!ELEMENT width (#PCDATA)>
<!ELEMENT height (#PCDATA)>
<!ELEMENT description (#PCDATA)>

+Vytvoril ukážkovú preznetáciu o ovocí pomocou xml.
+Vytvoril som XSLT pre konverziu zo xml do xhtml.
+Vytvoril som si vlastný CSS súbor.
