---
layout: post
title: "WYSIWYG oder Markdown"
date: 2012-04-05 06:19
comments: true
categories: 
---
Textverarbeitung ist eine ureigene Aufgabe für den Computer. Mit dem WYSIWYG-Ansatz nimmt man direkte Absatz- und Zeichenformatierungen vor und sieht dabei sofort das Ergebnis auf dem Bildschirm so, wie das Ergebnis aussehen wird. Auch Online-Dokumente (Webseiten und E-Mails) können mit WYSIWYG-Editoren erstellt. Doch was ist die Alternative?

Ein Hacker erstellt seine Texte gern in einem einfachen Texteditor. Für die Formatierung würde sich HTML eignen, wenn da nicht diese hässlichen <Tags> wären. Es muss aber auch nicht gleich das komplexe [LaTeX](http://de.wikipedia.org/wiki/LaTeX "Wikipedia zu LaTeX") sein, denn es gibt auch eine ganze Reihe vereinfachter Auszeichnungssprachen, die für das menschliche Auge leicht lesbar sind. Die größte Verbreitung scheint mir dabei **Markdown** zu haben.

Markdown nutzt sehr einfache Formatierungen, die einigen aus Nur-Text-E-Mails geläufig sein werde:
	**fett**, _kursiv_
	## Überschrift der 2. Ebene
	* Aufzählung
	1. Nummerierte Aufzählung
Dazu kommen noch einige Konzepte für Online-Dokumente, z. B.:
	[Linktext](URL "Optionaler Titel")
	![alt text](/path/to/img.jpg "Optionaler Titel")
Textblöcke beginnen mit 4 Leerzeichen oder einem Tab. Tabellen werden im Basic-Markdown nur mit Inline-HTML unterstützt, aber auch mit Markdown-Erweiterungen wie [PHP Markdown Extra](http://michelf.com/projects/php-markdown/extra/#table) oder [kramdown](http://kramdown.rubyforge.org/syntax.html#tables). Eine vollständige Dokumentation zu den Markdown-Basics findet man auf [daringfireball.net](http://daringfireball.net/projects/markdown/basics) oder auf deutsch: [markdown.de](http://markdown.de/syntax/).

**Auch diese Text wurde in Markdown geschrieben!** Octopress generiert die Blogbeiträge aus Markdown-Texten.

Besonders in der OpenSource-Szene (auf github) erfreut sich Markdown großer Beliebtheit. Markdown-Dokumentationen können profitieren von Versionierung genauso wie Quellcode. Der Vergleich oder ein Merge von zwei Dokumenten ist einfach möglich. Es eignet sich also auch für die kooperative Erstellung von Dokumentionen.