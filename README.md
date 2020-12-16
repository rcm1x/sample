Блок кода <!-- recommendix widget/ --> ниже надо вставить в шаблон сайта, между тегами <head>, код сам определит на каких страницах запускать виджет

этот код инициализирует виджет:

```
rcm1x(<код партнёра>, 'init', {
  position:'bottom-right',
  size:'m',
  wa:'<телефон поддержки в whatsapp, если есть>',
  tg:'<ссылка на группу в telegram, если есть>'
});
```

возможные значения параметров:

```
position?: 'bottom-right' | 'bottom-left' | 'top-left' | 'top-right'
size?: 's' | 'm' | 'l'
wa?: '+7[0-9]{10}'
tg?: string
```