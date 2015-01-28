# Pandoc

## Einführung

Gerade bei sehr großen LaTeX-Dokumenten kann das Schreiben eines Textes in LaTeX zu einer wahren Herausforderung werden. Denn die Syntax macht es nicht gerade einfach den Text zu erstellen und zu bearbeiten. Mit ***Markdown*** gibt es eine einfache Möglichkeit der Erstellung von Artikeln, Büchern, etc. Die Frage ist aber, wie man die Markdown-Dokumente für LaTeX nutzen kann. Anwendungen wie beispielsweise *Byword* haben eine entsprechende Exportfunktion. Doch nicht jeder Autor hat dieses Programm oder möchte es als Editor nutzen. Hier kommt **Pandoc** ins Spiel. Es  handelt sich dabei um ein Dokumenten-Konverter führ zahlreiche Formate, u.a. auch Markdown und LaTeX. 

## Pandoc installieren

Pandoc kann kostenlos [bei Github][] heruntergeladen werden. Es existieren Versionen für *Windows*, *Mac OS X* und *Linux*. Für die Verwendung ist außerdem eine LaTeX-Installation erforderlich. Die [Homepage][] des Pandoc-Entwicklers *John MacFarlane* enthält dazu weitere Informationen.

[bei Github]: https://github.com/jgm/pandoc/releases
[Homepage]: http://johnmacfarlane.net/pandoc/installing.html

## Pandoc nutzen

Die Umwandlung eines Markdown-Dokuments in ein LaTeX-Dokument ist denkbar einfach; die Syntax lautet:

	pandoc input.md -o output.tex

Die von Pandoc unterstützten Ein- und Ausgabeformate können mit folgender Syntax spezifiziert werden:

	pandoc -f markdown -t tex input.md > output.tex

Die Optionen stehen dabei für

	-f = from
	-t = to

Über die unterstützten Formate gibt [folgende Internetseite][] Aufschluss.  

[folgende Internetseite]: http://johnmacfarlane.net/pandoc/README.html

