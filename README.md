Zen Coding — a new way of writing HTML and CSS code
Follow us on Twitter @zen_coding

New version 0.7 is available (March 13, 2011), read release notes for more info.
Zen Coding is an editor plugin for high-speed HTML, XML, XSL (or any other structured code format) coding and editing. The core of this plugin is a powerful abbreviation engine which allows you to expand expressions—similar to CSS selectors—into HTML code. For example:

div#page>div.logo+ul#navigation>li*5>a
...can be expanded into:

<div id="page">
        <div class="logo"></div>
        <ul id="navigation">
                <li><a href=""></a></li>
                <li><a href=""></a></li>
                <li><a href=""></a></li>
                <li><a href=""></a></li>
                <li><a href=""></a></li>
        </ul>
</div>
Read more about current Zen Coding syntax

Abbreviation engine has a modular structure which allows you to expand abbreviations into different languages. Zen Coding currently supports CSS, HTML, XML/XSL and HAML languages via filters.

Current features of abbreviation engine
ID and CLASS attributes: div#page.section.main.
Custom attributes: div[title], a[title="Hello world" rel], td[colspan=2].
Element multiplication: li*5 will output <li> tag five times.
Item numbering with $ character: li.item$*3 will output <li> tag three times, replacing $ character with item number.
Multiple '$' characters in a row are used as zero padding, i.e.: li.item$$$ → li.item001
Abbreviation groups with unlimited nesting: div#page>(div#header>ul#nav>li*4>a)+(div#page>(h1>span)+p*2)+div#footer. You can literally write a full document markup with just a single line.
Filters support
div tag name can be omitted when writing element starting from ID or CLASS: #content>.section is the same as div#content>div.section.
(v0.7) Text support: p>{Click }+a{here}+{ to continue}.
To better understand how Zen Coding works, watch demo video and read Smashing Magazine tutorial.

Zen Coding isn’t only a decent abbreviation engine, it also provides some very useful actions for HTML-coder’s every day needs, like: Wrap with Abbreviation, Tag Balancing, Toggle Comment, Remove Tag etc. Read more about available actions.

Officially supported editors
These plugins are developed by Zen Coding team and guarantee to have full support of all Zen Coding latest features.

Aptana/Zend Studio/Eclipse (crossplatform) https://github.com/sergeche/eclipse-zencoding
TextMate (Mac). Available in two flavors: basic snippets (Zen HTML and Zen CSS) and full-featured plugin (ZenCoding for TextMate). Bundles > Zen Coding menu item
Coda (Mac) — external download, via TEA for Coda. Plug-ins > TEA for Coda > Zen Coding menu item
Espresso (Mac) — external download, via TEA for Espresso. Zen Coding is bundled with Espresso by default, but you should upgrade ZC to latest version. Actions > HTML menu item
Komodo Edit/IDE (crossplatform) — external download. Tools > Zen Coding menu item
Notepad++ (Windows). Zen Coding menu item Also a Python version of NPP plugin is available: http://sourceforge.net/projects/npppythonscript/files/
PSPad (Windows). Scripts > Zen Coding menu item
<textarea> (browser-based). See online demo.
editArea (browser-based). See online demo.
CodeMirror (browser-based). See online demo.
CodeMirror2 (browser-based). See online demo.
Third-party supported editors
These plugins are using official Zen Coding engine and developed by third-party developers. Thus, no guarantee that they support all latest ZC features.

Dreamweaver (Windows, Mac)
Sublime Text (Windows)
Sublime Text 2 (crossplatform) — install it from Package Control
UltraEdit (Windows)
TopStyle (Windows)
GEdit (crossplatform) — Franck Marcia's plugin, Mike Crittenden's plugin
BBEdit/TextWrangler (Mac) — external download
Visual Studio (Windows) — at Visual Studio Gallery
EmEditor (Windows) — external download
Sakura Editor (Windows) — external download
EditPlus (windows) — external download, release notes
NetBeans (crossplatform) — download
Chrome Extension — external download
Userscript for Greasemonkey — external download
Geany — external download
RJ TextEd — built in since v7.50
AkelPad — external download
WIODE web-based IDE
BlueFish — built-in in v2.2.1
Codelobster PHP Edition — built-in in v4.3
ShiftEdit — online IDE
Unofficial implementations
These plugins are developed by third-party and has their own ZC engine implementation, which leads to different feature set and abbreviation syntax. Zen Coding team has no relation to this projects.

IntelliJ IDEA/WebStorm/PHPStorm (crossplatform) — built-in in latest versions
Emacs (crossplatform) — external download
Vim (crossplatform) — Sparkup, Zen Coding for Vim
ReSharper plugin for Visual Studio
Development
Zen Coding is currently developed at GitHub. There’s also available developer previews of upcoming features and a Plugin HOWTO about adding Zen Coding support for your favorite editor. New Zen Coding releases are announces on our Twitter account.
