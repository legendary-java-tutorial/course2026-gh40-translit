# translit

Переводит кириллицу латиницей — команда в терминале и библиотека для Node.js. По умолчанию у меня ISO 9: одна латинская буква на каждую русскую, поэтому слово однозначно читается обратно.

Проект из шаблона курса GitHub 2026 JavaRush: код в `src/` — от курса, мои правки — алфавит в `translit.config.json` и этот README.

## Как запустить

Нужен Node.js 24.12 или новее.

```bash
npm install
npm start -- "Привет, жёлтый щенок"
npm start -- --list
npm test
```

## Мой алфавит

В `translit.config.json` выбран `iso9`:

```json
{
  "alphabet": "iso9"
}
```

«Привет, жёлтый щенок» → `Privet, žëltyj ŝenok`. Паспортным алфавитом вышло бы `Privet, zheltyi shchenok`.
