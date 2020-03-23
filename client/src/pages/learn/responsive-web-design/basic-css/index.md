---
title: Introduction to Basic CSS
block: Basic CSS
superBlock: Responsive Web Design
---
## Introducere in bazale CSS

Cascading Style Sheets (CSS) îi spune browser-ului cum să afișeze textul și alt conținut pe care îl scriem în HTML.

Ai grijă, CSS-ul este `case-sensitive`, literele majuscule diferă de cele minuscule.
Ca regula generala in CSS se scrie cu litere minuscule (a-z)

CSS a fost adoptat de toate browser-ele majore și îți permite să controle următoarele:

- culoarea (eng: color)
- fontul (eng: fonts)
- poziționarea (eng: positioning)
- spațierea (eng: spacing)
- dimensiune ale textului si conținutului (eng: sizing)
- decorații ale textului: italic, bold (eng: decorations)
- tranziții (eng: transitions)
  
Există 3 feluri principale de a folosi stilizarea CSS. Poti aplica stilurile direct pe elementele HTML (eng: `inline`) cu ajutorul atributului `style`. Alternativ, poti plasa regulile CSS in interiorul elementului `style` din documentul HTML. Al treilea mod este scrierea regulilor CSS intr-ul fisier de styluri (eng: style sheet) extern, care mai apoi este mentionat in documentul HTML. Chiar daca primele 2 moduri isi au intrebuintarile lor, majoritatea programatorilor prefera sa foloseasca style sheets externe pentru ca astfel pot tine regulile CSS separat de elementele HTML. Acest mod imbunatateste lizibilitatea (eng: readability) si reutilizabilitatea (reusability) codului tau.

Idea din spatele CSS este ca poti folosi un selector (eng: selector) ca sa tintesti un element HTML din DOM (Document Object Model) and mai apoi sa aplici diferite proprietaro pe acel element ca sa schimbi modul cum este afisat in pagina.

In aceasta sectiune o sa vezi cum adaugand reguli de stil CSS (eng: CSS styles) elementelor din CapPhotoAPP, poate transforma site-ul dintr-un text simplu in ceva mai mult. 
