---
layout: post
title:  "ByeBye, Octopress! Migration zu Jekyll!"
date:   2026-06-29 19:51:01 +0200
categories: jekyll migration
---
14 Jahre später kümmer ich mich doch nochmal 
um dieses Projekt. Es nach nur drei Beiträge 
(eigentich nur 2 und ein angefangener Git-Beitrag) 
habe ich das Projekt aufgegeben und einfach online 
gelassen.

Octopress wurde alt und inzwischen eingestellt. Mein Snyk-Scan berichtet wöchentlich per E-Mail eine Reihe von CVEs, zuletzt `1C 24H 20M 1L` (CVSS mit den 4 Stufen, Critical/High/Medium/Low - kurz C/H/M/L). 

Das habe ich jetzt geändert und im _Chat_ mit [Cloude Sonnet 4.6 (niedrig)](https://www.kiberatung.de/blog/claude-sonnet-4-6-alles-was-du-wissen-musst-deutsch?utm_medium=website) das alte Octopress-Projekt betrachtet, 
Alternativen wie `Hugo`, `Astro` und `Èleventy` ausgeschlossen und auf **Jekyll** migriert.

Wenn dieser Post online ist, hat das erfreulich 
gut geklappt. Am Ende habe ich noch den 
Beispiel-Post "Welcone to Jekyll" von Hand übersetzt 
(und dabei nochmal das Gelernte vertieft). 
Also folgendes:

Die Posts erstellt mal als Datei im `_posts`-Verzeichnis. Das Beispiel kann angepasst weden und nach einem Re-Build können die Änderungen betrachtet werden. Der Rebuild der Site kann auch verschienden Wegen passiernen, aber der übliche Weg ist das Ausführen von `jekyll serve` in der Command Line (CMD, Shell), was direkt auch einen Webserver startet und die Site bei jeder Änderung einer Datei neu generiert (auto-regenerates).

Jekyll benötigt Blogpost-Dateien, die in folgenden Format benannt werden:

`YEAR-MONTH-DAY-title.MARKUP`

Dabei ist `YEAR` eine 4-Ziffernnummer, `MONTH` und `DAY` sind beide 2-Ziffernnummern, und `MARKUP` ist die Dateierweiterung (file extension), die das benutzte Format der Datei repräsentiert. 

Jekyll bietet auch mächtigen Support für Code-Snippets:

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Lisa')
#=> prints 'Hi, Lisa' to STDOUT.
{% endhighlight %}

Besuch die [Jekyll docs][jekyll-docs] für mehr Infomationen,  um das meiste aus Jekyll herauszuholen. Bugs/Feature-Anforderungen können alle auf [Jekyll’s GitHub repo][jekyll-gh] eingebracht werden. Bei Fragen, kannst du auf [Jekyll Talk][jekyll-talk] fragen.

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
