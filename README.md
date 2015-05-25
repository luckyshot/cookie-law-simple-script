
Cookie Law simple script
===================================

Works IE8+.

Usage
-----------------------------------

Paste this code just before closing the <code>body</code> tag:

<pre>&lt;style&gt;#cookie-law-div{position:fixed;bottom:0;left:0;margin:0;padding:1em;width:100%;background:rgba(0,0,0,.5);color:#fff;font-size:80%}#cookie-law-div p{margin:0;text-align:center}#cookie-law-div button{position:fixed;right:1em;bottom:1em;background:0 0;border:none;color:#fff;opacity:.66;cursor:pointer}&lt;/style&gt;&lt;script&gt;cookieLaw={dId:"cookie-law-div",bId:"cookie-law-button",iId:"cookie-law-item",show:function(e){if(localStorage.getItem(cookieLaw.iId))return!1;var o=document.createElement("div"),i=document.createElement("p");b=document.createElement("button"),i.innerHTML=e.msg,b.id=cookieLaw.bId,b.innerHTML=e.ok,o.id=cookieLaw.dId,o.appendChild(i),o.appendChild(b),document.body.insertBefore(o,document.body.lastChild),b.addEventListener("click",cookieLaw.hide,!1)},hide:function(){document.getElementById(cookieLaw.dId).outerHTML="",localStorage.setItem(cookieLaw.iId,"1")}},cookieLaw.show({msg:"This site uses cookies to make the site simpler.",ok:"&amp;times;"});&lt;/script&gt;</pre>

That's it.

License
-----------------------------------

Public Domain.