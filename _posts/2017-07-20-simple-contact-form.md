---
inFeed: true
description: >-
  This looks like a simple contact form, yet it works really great on grid
  sites. The size is responsive - have a look at the page on your mobile, and
  the form is secure, using the Google reCaptcha.. the form is from a company
  called Formlets.
dateModified: '2017-08-30T13:27:17.914Z'
datePublished: '2017-08-30T13:27:18.270Z'
title: Simple Contact form..
author: []
publisher: {}
via: {}
hasPage: true
sourcePath: _posts/2017-07-20-simple-contact-form.md
starred: false
datePublishedOriginal: '2017-07-20T10:07:02.068Z'
url: simple-contact-form/index.html
_type: Article

---
# Simple Contact form..

This looks like a simple contact form, yet it works really great on grid sites. The size is responsive - have a look at the page on your mobile, and the form is secure, using the Google reCaptcha.. the form is from a company called [Formlets][0].

When you create an account on their site, there are all manner of form templates, blank forms, and all easily customizable. Change the colors, fonts, and logos.. easy..

The benefit of Formlets, apart from easy integration to a grid site, is that you can get one form for free! Most people will probably only need a contact form on their site, if you need more forms, you're likely to be a business.

Pricing can be found [here][1], for a small business for $180/yr you can have up to 10 forms, plenty to keep you going. This will also give you the ability to use **Paypal & Stripe** payment options.

To integrate the form into your grid site, we're going to use the supplied iframe code, and paste it into an embedded html window.

The code looks like :

    <script type="text/javascript" src="https://formlets.com/static/js/iframeResizer.min.js"></script>
    <iframe id="formlets-iframe" src="https://formlets.com/forms/tFvkEK8Dl2h1HKET/?iframe=true" frameborder="0" width="100%"></iframe>
    <script type="text/javascript" src="https://formlets.com/static/js/iframe.js"></script>

Now we're going to make a couple of simple changes. Remove the 2 lines that start with <script type=.... For the line that starts with <iframe id=.. we're going to add a height setting and change ?iframe=true to ?iframe=true&v=1

The height setting is going to be based on your form, and adding &v=1 stops the page autofocusing on the form. ie if the form is at the bottom of your page, it will prevent auto scrolling down to the form when a site visitor enters the page.

So our final embedded code to get the contact form working on our site is :

    <iframe id="formlets-iframe" src="https://formlets.com/forms/tFvkEK8Dl2h1HKET/?iframe=true&v=1" frameborder="0" width="100%" height="700"></iframe>

To prevent a vertical scroll bar in the embedded html window, we always make the size of the window to 10 more than the form height. The form below took less than 5 min to setup from creation to embed..

<iframe src="https://the-grid.github.io/ed-userhtml/?g=eJw1i0EKwjAQAL8SFvSm2XhRpFsvVoRe_YA2WxNsiGzW-n2hwePMME0c5Z7YRE8wZkkTa9lUB6bIQBBU3-Vo7b9uh5wWKFYv86vrD-dpF9y17272VE9S-fB6Jgdm4UcWz0KAYL7RayBwiCswgeMzKMEeEdrG1rn9AcvEMQ4" height="710" style=""></iframe>



[0]: https://formlets.com/?ref=gridtalk
[1]: https://formlets.com/pricing/?cur=USD&mode=YEARLY