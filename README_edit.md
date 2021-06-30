Jak editovat web?
=================

Markdown
--------

- Markdown je formát `.md` souborů, popř. je možný i HTML s většími možnostmi formátování.
- Online editor: https://markdown-editor.github.io
- Základy: https://www.markdownguide.org/cheat-sheet
- K vytištění: https://guides.github.com/pdfs/markdown-cheatsheet-online.pdf


Jak editovat existující stránku?
-------------------------------

- Každá stránka má dole odkaz `Editovat tuto stránku`.
- Přesměruje na GitHub, kde je vpravo nahoře ikona tužky `Edit this file`. (Je třeba se přihlásit pokud není.)
- Nebo ji najít ručně v adresářové struktuře na https://github.com/nulovapozice/nulovapozice.github.io.
- Editovat, případně je nahoře i `Preview changes`, a pak dole kliknout na `Commit changes`.


Jak přidat obrázek?
-------------------

- V grafickém editoru je třeba si nejdřív připravit obrázek.
    - Obrovské fotky zmenšit např. na velikost 1000 px.
    - Online editor je např. na https://www.photopea.com.
- V adresáři s obrázky https://github.com/nulovapozice/nulovapozice.github.io/tree/master/img nebo v nějakém jeho podadresáři kliknout na `Add file` a `Upload files`.
- Do libovolné stránky se pak můžou přidat pomocí následujícího kódu.

```markdown
![titulek](cesta k obrázku)

![Pozvánka](/img/posts/belarus-debata4-2048x1152.jpg)
```

Popř. embedded HTML bez odkazu/s odkazem...

```html
<img src="/img/posts/belarus-debata4-2048x1152.jpg" width="682" height="384" alt="Pozvánka" />

<a href="/img/posts/belarus-debata4-2048x1152.jpg">
  <img src="/img/posts/belarus-debata4-2048x1152.jpg" width="682" height="384" alt="Pozvánka" />
</a>
```


Čeština/ruština
---------------

Jazykové mutace jednotlivých stránek:

- https://github.com/nulovapozice/nulovapozice.github.io/tree/master/cz/
- https://github.com/nulovapozice/nulovapozice.github.io/tree/master/ru/


Překlady řetězců, co jsou různě po webu:

- https://github.com/nulovapozice/nulovapozice.github.io/blob/master/_data/lang.yaml


Jak přidat novou stránku?
-------------------------

- Na https://github.com/nulovapozice/nulovapozice.github.io je vidět adresářová struktura, najít správné místo.
- Nahoře kliknout na `Add file`, `Create new file`. (Je třeba se přihlásit pokud není.)
- Nahoře zadat jméno souboru, většinou s příponou `.md`. 
- Vytvořit obsah. Nejjednodušší bývá přes schránku zkopírovat něco existujícího, co má podobnou strukturu a upravovat.
- Dole kliknout na `Commit new file`.


Jak přidat novinku?
-------------------

- Úplně stejně jako novou stránku.
- Jsou v adresáři https://github.com/nulovapozice/nulovapozice.github.io/tree/master/cz/_posts.
- Jméno souboru má strukturu `YYYY-MM-DD-kratky-popis.md`, např. `2020-01-21-masopust.md`.
- Nahoře je hlavička a pak už jenom text, který se zobrazí.

```
---
layout: post
title: "Člověk a politika"
subtitle: "První cyklus workshopů v rámci divadelně-sociologického projektu"
background: '/img/posts/06.jpg'
lang: cz
---

Od září do prosince 2020 jsme zrealizovaly první cyklus workshopů...
```
