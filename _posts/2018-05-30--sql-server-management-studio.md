---
layout: post
published: true
title: پاک کردن تاریخچه اتصال به سرور در sql server management studio
subtitle: چگونه رد اتصال خود در MSMSرا پاک کنیم
date: '2018-05-30'
---
## پاک کردن تاریخچه اتصال به سرور در sql server management studio

اگر جایی توسط sql server management studioبه سروری متصل شده باشید، حتمی میدونید که اطلاعات اتصال شما به غیر از رمز عبور ذخیره میشن تا بعدا لازم نباشه تا مجدد تایپ کنیدش.

اگر دوست نداشتید اون اطلاعات اونجا بمونه یک راه حل وجود داره.

به مسیر زیر برید :

```
%APPDATA%\Microsoft\SQL Sever Management Studio\{your msms ver}\
```

 و فایل
 ```
 SqlStudio.bin
 ```
 
 رو پاک کنید.