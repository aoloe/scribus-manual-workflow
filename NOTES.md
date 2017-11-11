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

### "Collaborative editing"

Using the same Scribus document on multiple computers at the same time is not possible.

As with most type of files, Scribus files can only be edited by one person at a time.

### Sharing a document

The basic rule is: you cannot use the same Scribus document (from a shared disk or a usb key) on multiple computers.  
You have to collect the document for outpupt ("File > Collect for output") and you can then move the resulting directory to a different computer.

Directly sharing a Scribus document will sometimes work for some documents or parts of a document, but there is no guarantee that it will work for a whole document or for any specific document.  
There are workarounds that can let you share your work in well defined cases (see below for more details), but it won't in the general case.

Before we look further on ways to share the document, it's important to know what "collecting for output" does:

- The "biggest" task is to make sure that the document does not use absolute paths (in the form "D:\Documents\" or "/Volume/Work") to reference the images linked from your document. This is achieved by copying all images into the target directory.
- On top of this, it can also copy the font files and color profiles to ensure that the same resources are used.

The are two types of collaborations on a Scribus document:

- Each person does a specific task and then hands over the document to the next one for further procssing.
- Multiple persons edit the same document at different times.

In both cases the most straight forward way of sharing the document is to "collect for output" before handing over to the other person or putting it in the shared directory.

In the second case, where the document is shared "back and forth", this can become inpractical. If you are in control of all computers from where the document is accessed, you can of course try to make all the computers "look the same":

- All external images are linked to directories that have the exact same full path (starting from the  `C:` in Windows or the `/` on Linux or Mac)
  - This should be possible if all computers use the same operating system.
  - It's not possible to share a document between Windows and Mac or Linux.
  - It's possible but not trivial to share a directory between Mac and Linux.
- All computer should have the exact same fonts (same files, not only same names!) and all needed color profiles.

For "advanced" / corporate cases it should be possisble to create tools that modifiy the sla to make sure that the Scribus document can be used by multiple. This can be done from inside of Scribus with scripts or outside of it with by "cleaning up" the `.sla` file.

### Splitting the document in sections

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
