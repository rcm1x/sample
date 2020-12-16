Ссылка на пример интеграции виджета: [https://rcm1x.github.io/sample/wizard](https://rcm1x.github.io/sample/wizard)

Исходный код примера: [https://github.com/rcm1x/sample/blob/master/wizard.html](https://github.com/rcm1x/sample/blob/master/wizard.html)


Блок кода ниже, необходимо вставить в шаблон магазина, между тегами ```<head>```

Алгоритмы сервиса, самостоятельно определят, на каких страницах стоит показать пользователю виджет


Код подключения и инициализации виджета:

```html
<!-- recommendix widget -->
<script type="text/javascript">
  (function(r,e,c,o,m,me,n,d,i,x){
    r[m]=r[m]||function(){(r[m].i=r[m].i||[]).push(arguments)},
    me=e.createElement(c),x=e.getElementsByTagName(c)[0],me.async=1,
    me.src=o,x.parentNode.insertBefore(me,x)
  })(window,document,'script','https://rcm1x.me/i/tag.js','rcm1x');

  rcm1x(<код_партнёра>, 'init', {
    position:'bottom-right',
    size:'m',
    wa:'<телефон поддержки в whatsapp, если есть>',
    tg:'<ссылка на группу в telegram, если есть>'
  });
</script>
<!-- /recommendix widget -->
```


Возможные значения параметров:

```JS
position?: 'bottom-right' | 'bottom-left' | 'top-left' | 'top-right'
size?: 's' | 'm' | 'l'
wa?: '+7[0-9]{10}'
tg?: string
```

Техническая поддержка и помощь в подключении: [support@recommendix.com](mailto:support@recommendix.com)
