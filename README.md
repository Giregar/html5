# HTML5

<h2><span style="color: #e98b38;">1. Was ist HTML?</span></h2>
HTML bedeutet <strong>H</strong>yper<strong>t</strong>ext&nbsp;<strong>M</strong>arkup&nbsp;<strong>L</strong>anguage. Mit einer Markup Language können wir Schlüsselwörter (Tags) verwenden, um ein HTML Dokument (Website) zu strukturieren. Die unterschiedlichen Tags und die dazugehörigen Funktionen, werden wir im Laufe dieses Artikels näher betrachten.
<h2><span style="color: #e98b38;">2. Was sind Tags?</span></h2>
Wir strukturieren unsere Website mit Tags. Diese verwenden Schlüsselworte wie&nbsp;<strong>body</strong>,&nbsp;<strong>form</strong> oder&nbsp;<strong>i </strong>beinhalten. Viele Tags besitzen auch einen sogenannten&nbsp;<em>abschließenden Tag</em>.&nbsp;Anbei ein Beispiel:
<pre class="lang:html decode:true">&lt;tagname attribut=""&gt;Content&lt;/tagname&gt;
</pre>
Der abschließende Tag beinhaltet einen Schrägstrich. Einige Tags haben bestimmte Attribute, die wir genauer definieren können.
<h2><span style="color: #e98b38;">3. Welchen Editor?</span></h2>
Wenn wir nun unser erstes HTML Dokument schreiben wollen, wählen wir einen Editor unserer Wahl. Ich verwende den kostenlosen Editor&nbsp;<a href="https://www.sublimetext.com/3">Sublime Text 3</a>. Diesen werde ich auch in allen zukünftigen Beispielen verwenden. Zu Beginn reicht es aber aus, den einfachen Editor (Windows) oder TextEdit (OSX) zu verwenden. Am Ende kommt es nur darauf an, dass wir dem Dokument beim speichern das Dateiform&nbsp;<strong>.html&nbsp;</strong>geben können.
<blockquote><strong>Tipp:</strong> Du kannst statt eines Texteditors auch eine IDE (Integrierte Entwicklungsumgebung) verwenden.&nbsp;Eine solche IDE bietet viele nützliche Funktionen, wie das Darstellen von HTML Dokumenten, direkter Upload via integrierten FTP Client und noch vieles mehr. Eine weit verbreitete IDE ist&nbsp;Eclipse.</blockquote>
<h2><span style="color: #e98b38;">4. Das Grundgerüst</span></h2>
Nun kommen wir zu dem HTML Grundgerüst, welches wie folgt aussieht:
<pre class="lang:html decode:true">&lt;!doctype html&gt;
&lt;html&gt;  
  &lt;head&gt;
    &lt;title&gt;Page title&lt;/title&gt;
  &lt;/head&gt;
  &lt;body&gt;
    &lt;!-- Dies ist ein Kommentar --&gt;
    Hello World
  &lt;/body&gt;
&lt;/html&gt;</pre>
Im &lt;html&gt; Tag haben wir den Typ unseres Dokuments mit&nbsp;<strong>!doctype html</strong> angegeben. Einige Browser benötigen diese Information, außerdem gehört es zum guten Stil, einen Doctype zu verwenden.&nbsp;Innerhalb der &lt;html&gt; Tags sehen wir nun zwei Bereiche: Den&nbsp;<strong>head</strong> und den&nbsp;<strong>body</strong> Bereich. Wenn wir diesen Code-Snippet nun in unseren Editor einfügen und als <strong>index.html</strong> abspeichern, können wir sie danach mit einem beliebigen Browser öffnen.
<blockquote><strong>Tipp:</strong> Solltest du einen Texteditor verwenden, der nativ keine Dokumente mit der Endung .html abspeichern kann, dann wähle beim Speichern als Dokumenttyp "Alle Dateien" und füge beim Dateinamen die Endung .html hinzu.</blockquote>
<ul>
 	<li>Zwischen den <strong>&lt;head&gt;</strong> Tags haben wir die Möglichkeiten, weitere Informationen der Website zu definieren.</li>
 	<li>Der im Browser sichtbare Teil der Website, steht zwischen den&nbsp;<strong>&lt;body&gt;</strong> Tags .</li>
 	<li>Kommentare werden zwischen&nbsp;<strong>&lt;!--</strong>&nbsp;Hier steht ein Kommentar<strong>&nbsp;--&gt;</strong> geschrieben. Diese werden nicht auf der Website zu sehen sein.</li>
</ul>
Lass uns jetzt die nötigen Tags angucken, um eine erste Website zu erstellen.
<h2><span style="color: #e98b38;">5. Überschriften:&nbsp;<em>&lt;h1&gt; bis &lt;h6&gt;</em></span></h2>
Es gibt sechs verschiedene Größen für die Überschriften. So ist die Überschrift zwischen den&nbsp;<strong>&lt;h1&gt;&lt;/h1&gt;</strong>&nbsp;Tags am größten und zwischen&nbsp;<strong>&lt;h6&gt;&lt;/h6&gt;</strong> am kleinsten. Überschriften werden nicht in Paragraphen eingebettet.
<h1>&lt;h1&gt;Überschrift&lt;/h1&gt;</h1>
<h2>&lt;h2&gt;Überschrift&lt;/h2&gt;</h2>
<h3>&lt;h3&gt;Überschrift&lt;/h3&gt;</h3>
<h4>&lt;h4&gt;Überschrift&lt;/h4&gt;</h4>
<h5>&lt;h5&gt;Überschrift&lt;/h5&gt;</h5>
<h6>&lt;h6&gt;Überschrift&lt;/h6&gt;</h6>
<h2><span style="color: #e98b38;">6. Absätze:&nbsp;<em>&lt;p&gt;</em></span></h2>
Absätze bzw. Paragraphen werden vom&nbsp;<strong>&lt;p&gt;&lt;/p&gt;</strong> Tag umschlossen. Ein Paragraph erzeugt nach Schließung&nbsp;einen Zeilenumbruch.
<pre class="lang:html decode:true">&lt;p&gt;This is my first paragraph.&lt;/p&gt;
&lt;p&gt;This is the second one.&lt;/p&gt;</pre>
<h2><span style="color: #e98b38;">7. Bilder: <em>&lt;img&gt;</em></span></h2>
Der &lt;img&gt; Tag hat keinen abschließenden Tag.

Wichtige Attribute:
<ul>
 	<li><strong>src</strong> gibt den Pfad zum Bild an.</li>
 	<li><strong>alt</strong> definiert&nbsp;einen alternativen Text. Dieser wird dargestellt, falls das Bild nicht geladen werden kann.</li>
 	<li><strong>height</strong> und&nbsp;<strong>width&nbsp;</strong>definieren die Höhe und Breite des Bildes.</li>
</ul>
<pre class="lang:html decode:true">&lt;img src="Pfad/zum/Bild" alt="Alternative Text" width="100" height="150"&gt;</pre>
<h2><span style="color: #e98b38;">8. Links:&nbsp;<em>&lt;a&gt;</em></span></h2>
Links verknüpfen HTML Dokumente oder lassen uns andere Websites aufrufen. In unserem Beispiel haben wir zwischen die &lt;a&gt; Tags den Text "This is a link" geschrieben. Der Link wird beim Aufrufen im Browser nun als dieser Text dargestellt.

Wichtige Attribute:
<ul>
 	<li><strong>href</strong> definiert unser Ziel.</li>
</ul>
<pre class="lang:html decode:true">&lt;a href="http://www.siregar.net"&gt;This is a link&lt;/a&gt;</pre>
<h2><span style="color: #e98b38;">9. Beispiel: Hallo Welt</span></h2>
Nun haben wir die nötigen Basics kennengelernt, um ein einfaches HTML Dokument zu erstellen. Wir werden nun eine erste Website erstellen, die eine Überschrift und einige Absätze beinhalten&nbsp;wird.&nbsp;Öffne nun den Texteditor deiner Wahl und füge den folgenden Code ein:
<pre class="lang:html decode:true">&lt;html&gt;
  &lt;head&gt;
    &lt;title&gt;Welcome&lt;/title&gt;
  &lt;/head&gt;
  &lt;body&gt;
    &lt;h1&gt;My first website&lt;/h1&gt;
    &lt;!-- First paragraph --&gt;
    &lt;p&gt;
      Lorem ipsum dolor.
      &lt;a href=""&gt;Link 1&lt;/a&gt;
    &lt;/p&gt;
    &lt;!-- Second paragraph --&gt;
    &lt;p&gt;
      Lorem ipsum dolor.
      &lt;a href=""&gt;Link 2&lt;/a&gt;
    &lt;/p&gt;
  &lt;/body&gt;
&lt;/html&gt;</pre>
Speichere deinen Quellcode nun als index.html ab und rufe sie über einen beliebigen Browser auf.&nbsp;Ändere die Texte und Links&nbsp;und füge vielleicht ein Bild mit dem &lt;img&gt; Tag ein.
<h2><span style="color: #e98b38;">10.&nbsp;Zusammenfassung</span></h2>
Wir haben in diesem Artikel das Grundgerüst einer Website kennengelernt. Es ist nun bekannt,&nbsp;wie&nbsp;wir mit den passenden Tags&nbsp;unsere Texte, Bilder und Links einfügen. Das sind aber noch nicht alle Möglichkeiten, die wir mit HTML haben. Im nächsten Artikel, werden wir uns mit der Formatierung des Inhalts einer Website beschäftigen.
