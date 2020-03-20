# javascript-storage

хелпер для работы с `localStorage`

### Установка
```shell
$ npm install javascript-storage
```

Надо настроить в вашем сервере резолв с `/javascript-storage` в `node_modules/javascript-storage`

```html
  <script type="importmap">
  {
    "imports": {
      "javascript-storage": "/javascript-storage/index.js"
    }
  }
  </script>
```

### Использование
```javascript
import Storage from 'javascript-storage';

const storage = new Storage();

storage.set(name, data); //
storage.get(name);       // data
storage.remove(name);    //
storage.clear();         //
```

### Дополнительно
Если вы используете vscode, можно настроить резолв для корректной работы самого редактора с помощью файла `jsconfig.json`
```json
{
  "compilerOptions": {
    "baseUrl": "../node_modules/",
    "paths": {
      "javascript-storage/*": ["./javascript-storage/*"]
    }
  }
}
```
