# Workflows für Scribus

## Preparing text for Scribus

die idee dein text in odt zu schreiben ist gut.

txt ist auch eine möglichkeit, aber odt hat schon ein paar vorteile.

im erwähnten fall (die listen!) liegt das problem eher bei scribus.
leider kennt scribus noch keine liste als solche. sie sind bereits programmiert aber noch nicht in der jetzige stabile version veröffentlicht.
die listen musst du also selber als eingerückte absätze in der formatvorlagen definieren. und bindenstrichen manuel einfügen.

also, doch, vielleicht gab es doch ein gedankenfehler: es lohnt sich nicht zu viel zeit im layout in libre/open-office zu investieren.
libreoffice ist da um text zu schreiben, und ein wenig grund vormatierung passt auch rein.
aber das layout erfolgt dann in scribus.

## Preparing images for Scribus

## Templates

If you downloaded a template from a place like scribusstuff (or otherwise got a template) open it as a normal `.sla` and `file > save as a template`.

## Files location hygiene

ne déplace ni renomme les dossier contenant des fichiers scribus ou leur ressources.

et quand tu fais une copie de sauvegarde, ne copie pas le dossier où se trouvent les fichiers, mais utilise "collect for output".

un dossier/fichier créé avec "collect for output" peut être déplacé, tant que tu ne l'as pas édité.

en général, il y a "deux façon de travailler":

- tu mets tout ce qui est actuel en premier plan et tu le déplace dans un archive lorsque c'est du passé ou
- tu places dès le début le fichier actuel au bon endroit et tu travaille toujours sur la version actuelle (les copies ne sont que pour l'archivage).

je voies beaucoup de monde autour de moi qui utilise le premier workflow. et je l'utilise aussi pour des projets qui ont une très courte durée (maximum 10 minutes... ensuite effacé).

dans mon cas, tout le reste est placé dès le début au bon endroit. pas seulement avec scribus.

le premier workflow permet probablement de mieux se concentrer sur ce qui est important, mais je remarques que ça pose souvent de gros problèmes:

- quelle est la version définitive / actuelle de mon document?
- où est mon fichier?

en tout cas, avec scribus il n'y a pas de choix: c'est le deuxième ou des gros maux de tête...

## Colaborating on a Scribus document

As with most type of files, Scribus files can only be edited by one person at a time.

Depending on your needs there are two ways of collaborating on a Scribus project.

### Working on the same document one person at a time

It's of course possible to have several people working on the same computer, one after the other.

 

### Spreading


laser hat dir bereits eine gute anleitung gegeben. sie wird dein problem lösen, wenn ihr nicht gleichzeitig arbeiten musst / wollt.

anderseits, falls

- jeder eine seite allein gestaltet,
- "unabhängig" von einander arbeiten möchtet

dann empfehle ich euch:

- ein einseitiges "musterdokument" zu erstellen (gemeindebriefe-17-01-00.sla), es für die ausgabe sammeln und allen zu verfügung stellen
- irgendwie eine liste verwalten, wo jeder trägt ein, welche seite er/sie übernimmt / übernehmen soll.
- jeder nimmt eine kopie vom musterdokument pro seite, benennt es um (z.b. gemeindebriefe-17-01-01.sla für die erste seite der januar ausgabe...), arbeitet drauf (ohne die formatvorlagen und musterseiten anzupassen!)...
- ... und wenn er/sie fertig ist, sammelt das resultat für die ausgabe und ladet es in eine gemeinsame ablage hoch.
- noch besser, jeder nimmt eine doppelseite... oder?
- am ende, ein.e koordinator-I-n fügt die seiten zusammen (seite > importieren)
- bitte vor dem gebrauch durchtesten : - )

es ist auch möglich ein pdf pro seite/dokument zu generieren und dann die PDFs zusammen zu fügen.
