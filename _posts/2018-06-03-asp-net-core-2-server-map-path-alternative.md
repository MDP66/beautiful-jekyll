---
layout: post
published: true
title: پیدا کردن root در asp.net core 2
subtitle: پیدا کردن root در asp.net core 2
---
## پیدا کردن root در asp.net core 2

در asp.net قبل از core برای پیدا کردن آدرس فیزیکی یک فایل از `Server.MapPath` استفاده می شد.

درساختار asp.net core دیگه خبری از Server نیست و باید از middleware های داخلی جهت دستیابی به امکانات قبلی استفاده کرد.

یکی از این middleware ها `IHostingEnvironment` هست.

در asp.net core برای پیدا کردن root می تونید از دستور زیر استفاده کنید

```C#
public class SampleController : Controller
{
	private IHostingEnvironment _env;
    public SampleController(IHostingEnvironment env)
    {
    	_env = env;
    }
    
    public async Task<IActionResult> GetMePath()
    {
    	return Content("path: " + _env.WebRootPath, "text/plain");
    }
}
```

> یه نکته خیلی کنکوری اینجا هست اونم اینه که اگر فولدر wwwroot پروژه وجود نداشته باشه، خروجی متند خالی خواهد بود.

