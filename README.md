<h2>JavaDoc Clean Read plugin for IntelliJ platform IDEs.</h2>

<h4>Why?</h4>
      HTML and JavaDoc <b>tags</b>, as well as HTML <b>escaped chars</b> make the text of JavaDoc comments <b>hard to read</b> (sometimes almost impossible) in the Code Editor.<br>    
     We can open the quick documentation window (Ctrl+Q or ⌃J or View > Quick Documentation from the menu). But that need additional actions and give the text formatted withing different style then source code. Also links at the JavaDoc comment lead to the source code of linked element, but at the quick documentation window it leads to generated JavaDoc of linked element, which is not what we usually desire.<br>

<h4>How?</h4>
      <li> Hiding(folding) HTML tags;
      <li> Unescape HTML escaped chars;
      <li> Apply appropriate text styles for value of tags: &lt;code&gt; | &lt;tt&gt; | &lt;li&gt; | &lt;b&gt; | &lt;i&gt; | @code | @link;
      <li> Some tag value text styles are customisable at Settings -> Editor -> Color Scheme -> JavaDoc Clean Read. <br>

Both HTML-JavaDoc tags hiding and HTML escaped chars unescaping are implemented through IntelliJ <a href="https://www.jetbrains.com/help/idea/code-folding.html">code folding</a>. So all shortcuts (Ctrl+. Ctrl+NumPad + and others) works. As well as <i>code folding toggles</i> (like <code>&#x2302;</code>) shown in the editor to the left of the corresponding multiline folding regions. <br>       

There are some limitations for corner cases in current release: multiline tags, nested tags, ... But mostly it works fine. <br>

Side by side comparison of <code>java.lang.String</code> top JavaDoc comment: <br>
<img src="Screenshot_String.png">

For even more fun see <code>java.util.regex.Pattern</code> ;) <br>
<img src="Screenshot_Pattern.png">
<h4>Alternatives?</h4>
    I don't know any... :( <br> Would be glad if JetBrain implements that more proper way as part of IntelliJ platform. 

## **License**

Plugin is open-source software and is licenced under GPL v3 licence.

## **Versions**
0.1.0 - Initial release: <br>
           &emsp; * hiding(folding) HTML tags; <br>
           &emsp; * unescape HTML escaped chars; <br>
           &emsp; * text styles for tags: &lt;code&gt; | &lt;tt&gt; | &lt;b&gt; | &lt;i&gt; | @code | @link. <br>
