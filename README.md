
Cookie Law simple script
===================================

One line of JavaScript that displays a Cookie Law message:

![cookie-law-message](https://cloud.githubusercontent.com/assets/141241/11879577/7d24dd98-a4fc-11e5-80a3-cb0c285f00e6.png)

- Works IE8+
- Multilanguage support
- Remembers when it has been closed

Usage
-----------------------------------

Paste this code just before the closing <code>&lt;/body&gt;</code> tag:

<pre>&lt;style&gt;#cookie-law-div{position:fixed;bottom:0;left:0;margin:0;padding:1em;width:100%;background:rgba(0,0,0,.5);font-size:80%}#cookie-law-div p{margin:0;text-align:center;color:#fff}#cookie-law-div button{float:right;line-height:1;font-size:24px;background:0 0;border:none;color:#fff;opacity:.66;cursor:pointer}&lt;/style&gt;&lt;script&gt;cookieLaw={dId:"cookie-law-div",bId:"cookie-law-button",iId:"cookie-law-item",show:function(e){if(localStorage.getItem(cookieLaw.iId))return!1;var o=document.createElement("div"),i=document.createElement("p"),t=document.createElement("button");i.innerHTML=e.msg,t.id=cookieLaw.bId,t.innerHTML=e.ok,o.id=cookieLaw.dId,o.appendChild(t),o.appendChild(i),document.body.insertBefore(o,document.body.lastChild),t.addEventListener("click",cookieLaw.hide,!1)},hide:function(){document.getElementById(cookieLaw.dId).outerHTML="",localStorage.setItem(cookieLaw.iId,"1")}},cookieLaw.show({msg:"This site uses cookies to make the site simpler.",ok:"&times;"});&lt;/script&gt;</pre>

That's it.



## Sample texts

### English

This site uses cookies to make the site simpler.

They force us to bother you with the obvious fact that this site uses cookies.

This website uses cookies. Cookies remember you so we can give you a better online experience.

We use cookies to give you the best possible experience. By continuing to visit or use our services, you agree to the use of cookies as described in our Cookie Policy.

We use cookies and other tracking technologies to improve your browsing experience on our site, show personalized content and targeted ads, analyze site traffic, and understand where our audience is coming from.

We use our own and third-party cookies to improve our services and show you advertising related to your preferences by analyzing your browsing habits. If you continue surfing, we will consider you are accepting its use.

We use cookies to understand how you use our site and provide the best browsing experience possible. This includes analysing our traffic, personalizing content and advertising. By continuing to use our site, you accept our use of cookies, Privacy Policy and Terms of Service.

We use cookies and similar technologies to measure traffic, repeat visitors and site performance. Learn more about cookies (including how to disable them). By clicking “I agree”, “X” or by continuing to use our site you consent to the use of cookies (unless you’ve disabled cookies).

We use cookies to ensure that we give you the best experience on our website. This includes cookies from third party social media websites if you visit a page which contains embedded content from social media. Such third party cookies may track your use of this website. We and our partners also use cookies to ensure we show you advertising that is relevant to you. If you continue without changing your settings, we'll assume that you are happy to receive all cookies on this website.


#### Affiliate link

We are reader-supported. If you click on or buy something via a link on this page, we may earn a commission.

You support our site by purchasing what we recommend.


### Spanish

Nos obligan a molestarte con la obviedad de que este sitio usa cookies.

Utilizamos cookies para mejorar su experiencia. Al continuar acepta las cookies y nuestra política de cookies.

Esta web utiliza cookies propias y de terceros para ofrecerle una mejor experiencia y servicio y poder registrar el proceso de compra. Al navegar o utilizar nuestros servicios el usuario acepta el uso que hacemos de las cookies.

Utilizamos cookies propias y de terceros para mejorar nuestros servicios y mostrarle publicidad relacionada con sus preferencias mediante el análisis de sus hábitos de navegación. Si continua navegando, consideramos que acepta su uso.
