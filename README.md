
Cookie Law simple script
===================================

One line of JavaScript that displays a Cookie Law message:

![cookie-law-message](https://cloud.githubusercontent.com/assets/141241/11879577/7d24dd98-a4fc-11e5-80a3-cb0c285f00e6.png)

- Works IE8+
- Multilanguage support
- Remembers when it has been closed

Usage
-----------------------------------

Paste this code just before closing the <code>body</code> tag:

<pre>&lt;style&gt;#cookie-law-div{position:fixed;bottom:0;left:0;margin:0;padding:1em;width:100%;background:rgba(0,0,0,.5);color:#fff;font-size:80%}#cookie-law-div p{margin:0;text-align:center}#cookie-law-div button{position:fixed;right:1em;bottom:1em;background:0 0;border:none;color:#fff;opacity:.66;cursor:pointer}&lt;/style&gt;&lt;script&gt;cookieLaw={dId:"cookie-law-div",bId:"cookie-law-button",iId:"cookie-law-item",show:function(e){if(localStorage.getItem(cookieLaw.iId))return!1;var o=document.createElement("div"),i=document.createElement("p");b=document.createElement("button"),i.innerHTML=e.msg,b.id=cookieLaw.bId,b.innerHTML=e.ok,o.id=cookieLaw.dId,o.appendChild(i),o.appendChild(b),document.body.insertBefore(o,document.body.lastChild),b.addEventListener("click",cookieLaw.hide,!1)},hide:function(){document.getElementById(cookieLaw.dId).outerHTML="",localStorage.setItem(cookieLaw.iId,"1")}},cookieLaw.show({msg:"This site uses cookies to make the site simpler.",ok:"&amp;times;"});&lt;/script&gt;</pre>

That's it.



## Sample texts

### English

This site uses cookies to make the site simpler.

We use cookies to ensure that we give you the best experience on our website. This includes cookies from third party social media websites if you visit a page which contains embedded content from social media. Such third party cookies may track your use of this website. We and our partners also use cookies to ensure we show you advertising that is relevant to you. If you continue without changing your settings, we'll assume that you are happy to receive all cookies on this website.

They force us to bother you with the obvious fact that this site uses cookies.


### Spanish

Utilizamos cookies para mejorar su experiencia. Al continuar acepta las cookies y nuestra política de cookies.

Esta web utiliza cookies propias y de terceros para ofrecerle una mejor experiencia y servicio y poder registrar el proceso de compra. Al navegar o utilizar nuestros servicios el usuario acepta el uso que hacemos de las cookies.

Nos obligan a molestarte con la obviedad de que este sitio usa cookies.
