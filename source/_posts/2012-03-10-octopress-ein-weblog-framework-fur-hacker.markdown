---
layout: post
title: "Octopress - Ein Weblog-Framework für Hacker"
date: 2012-03-10 19:07
comments: true
categories: [Octopress, Ruby, Github, Markdown]
published: true
---
Bei meiner Recherche zu Markdown bin ich zufällig über **Octopress** gestolpert, ein Blogging-System der etwas anderen Art. Es basiert nicht auf das übliche Set von PHP + MySQL, welches ein Web-CMS bietet. Nein, ganz im Gegenteil. [Octopress](http://octopress.org/) basiert Ruby und ein Git-Repository. Um mit Octopress zu arbeiten, klont man sich das dazugehörige Repository von [Github](https://github.com/imathis/octopress) und erzeugt einen Posting mit in der Kommandozeile.
	
	rake new_post["Mein neuer Blogposttitel"]


Generiert wird dadurch eine Markdown-Datei im Unterverzeichnis `source/_posts` nach der Konvention `YYYY-MM-DD-post-title.markdown`. Die Datei enthält dann etwa 7 Zeilen Metadaten in einem yaml-Header. Der Header von diesem Post sieht so aus:

```
	---
	layout: post
	title: "Octopress - Ein Weblog-Framework für Hacker"
	date: 2012-03-10 19:07
	comments: true
	categories: [Octopress, Ruby, Github, Markdown]
	---
```

Darunter schreibt man mit einem Texteditor seiner Wahl (textmate, vi, emacs, notepad++) den eigentlichen Blogpost in Markdown-Syntax. Octopress unterstützt dabei die erweiterte Syntax von kramdown.

Abschließend lässt man dann den fertigen Post als statische HTML-Seite generieren. Wie gesagt, keine Datenbank, kein Web-CMS!

	rake generate
	
Für das Hosting habe ich mich für eine _Github Page_ enschieden. Alternativ beschreibt die Octopress die Nutzung der Platform _Heroku_ oder einem eigenen Server, welcher mit _Rsync_ bestückt wird. Wenn man eine _Github Page_ erstmal eingerichtet hat genug für das Deployment:

	rake deploy
	
Github informiert jeweils per E-Mail, wenn die Seite erfolgreich neu erstellt wurde. Fertig.

Auf die Tools __Git/Github__, __Markdown__ und __ruby__ werde ich vielleicht in einem späteren Blogpost etwas genauer eingehen. Abschließend noch die Features, die mich bei _Octopress_ überzeugt haben.

* Modernes Webdesign mit HTML5
* Ein Template mit einem _Responsive Layout_
* Schreiben mit Markdown
* Einfache Plugins zur Erweiterung
* Einfaches Deployment

Ein Manko hat _Octopress_ natürlich. Da nicht mit einer Datenbank gearbeitet wird, kann auch mit Bordmitteln kein Kommentarformular angeboten werden, da Kommentare auch nirgendwo gespeichert werden könnten. Aber auch hier gibt es eine Plugin zur Kommentarplatform [Disqus](http://disqus.com/).