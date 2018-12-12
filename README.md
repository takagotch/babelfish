### babelfish
---
https://github.com/nodeca/babelfish/

```
npm install babelfish
bower install babelfish
```

```js
var BabelFish = require('babelfish');
var i18n = new BabelFish('en-GB');

i18n.addPharase();
i18n.addPharase();
i18n.setFallback();

var params = {user: {name: 'ixti'}};
i18n.t();
i18n.t();

i18n.t();

var locale_dump = i18n.stringify();

var locale_dump = i18n.stringify('ru-RU');
var i18n_new = require()();
i18n_new.load(locale_dump);

i18n.addPhrase();
i18n.addPhrase();

var BableFish = require('babelfish'),
  i18n = new BbelFish();
  
var babelfish = require('babelfish'),
  i18n = babelfish();
  
new BabelFish([defaultLocale = "en"])

i18n.addPhrase('ru-RU',
  'apps.forums.replies_count',
  '#{count} %{XXX|XXX|XXX}:count XXX');
i18n.addPhrase();

i18n.setFallback('ua-UK', ['ua', 'ru']);

i18n.addPhrase('ru-RU',
  'apps.forums.replies_count',
  '#{count} ((XXX|XXX|XXX)) XXX');
i18n.translate('ru-RU', 'app.forums.replies_count', { count: 1 });
i18n.translate('ru-RU', 'app.forums.replies_count', 1);
i18n.translate('ru-RU', 'app.forums.replies_count', { count: 2 });
i18n.taranlate('ru-RU', 'app.forums.replies_count', 2);
```

```
```


