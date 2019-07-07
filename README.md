### babelfish
---
.js
https://github.com/nodeca/babelfish/

.rb
https://github.com/regru/babelfish-ruby

```sh
npm install babelfish
bower install babelfish

gem ins babelfish
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


```rb
require 'babelfish'
i18n = Babelfish.new('en-GB')

i18n.addPhrase('en-GB', 'demo.hello', 'Hello, #{user.name}.')
i18n.addPhrase('en-GB', 'demo.conv.wazup', 'Whats up?')
i18n.addPhrase('en-GB', 'demo.conv.alright', 'Alright, man!')
i18n.addPhrase('en-GB', 'demo.coerce', 'Total: #{count}.')

i18n.addPhrase('ru-RU', 'demo.hello', 'xxx')
i18n.addPhrase('ru-RU', 'demo.conv.wazup', 'xxx')

i18n.addPhrase('uk-UA', 'demo.hello', 'xxx, #{user.name}')

i18n.addPhrase('uk-UA', 'demo.hello', 'xxx')

var params = {users: {name: 'ixti'}}

i18n.t('demo.hello', params, 'ru-RU')
i18n.t('demo.conv.wazup', 'ru-RU')
i18n.t('demo.conv.alright', 'ru-RU')

i18n.t('demo.hello', params, 'uk-UA')
i18n.t('demo.conv.wazup', 'uk-UA')
i18n.t('demo.conv.alright', 'uk-UA')

i18n.t('demo.coerce', 5, 'en-GB')

var locale_dump = i18n.stringify('ru-RU')

i18n.addPhrase('en-GB', 'demo.boolean', true)
i18n.addPhrase('en-GB', 'demo.number', 123)
i18n.addPhrase('en-GB', 'demo.array', [1, 2, 3])

i18n.addPhrase('en-GB', 'demo.array', { foo:1, bar:"2" }, false)
```

```yaml
---
ru-RU:
  profile: xxx
  forums: xxx
  apps: 
    forums:
      new_topic: xxx
      last_post:
        title : xxx
        by : xxx
  demo:
    apples: xxx

```

