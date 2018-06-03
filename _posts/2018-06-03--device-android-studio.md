---
layout: post
published: false
title: تغییر device پیش فرض در android studio
---
## چگونه device انتخاب شده در Android Studio را تغییر دهیم

در Android Studio ورژن 3.1 به بعد در هنگام دیباگ امکانی به پروژه اضافه شده که در صورتی که چندین Virtual Device و یا Connected Device داشته باشید، جهت کمتر نمایش داده شدن پنجره انتخاب device، می توان یک device را به عنوان پیش فرض انتخاب کرد.

مشکل به وجود آمده این امکان این است که در صورتی که لازم به تغییر device باشید، پنجره انتخاب device دیگر نمایش داده نمی شود.

برای رفع این حالت مراحل زیر را طی کنید :

``
Run menu -> Edit Configurations -> General Tab -> uncheck "use same device for future launches"
``

![change_build_target.png]({{site.baseurl}}/img/change_build_target.png)
