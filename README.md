# translit

Переводит кириллицу латиницей — команда в терминале и библиотека для Node.js. По умолчанию у меня немецкая транскрипция: так русские имена пишут в Германии — ж и ш дают sch, ч — tsch, х — ch.

Проект из шаблона курса GitHub 2026 JavaRush: код в `src/` — от курса, мои правки — алфавит `alphabets/german.json`, выбор в `translit.config.json` и этот README.

## Как запустить

Нужен Node.js 24.12 или новее.

```bash
npm install
npm start -- "Привет, жёлтый щенок"
npm start -- --list
npm test
```

## Мой алфавит

Свой алфавит — `alphabets/german.json`, копия паспортного с немецкими буквами; в `translit.config.json` выбран он:

```json
{
  "alphabet": "german"
}
```

«Привет, жёлтый щенок» → `Privet, scheltyi schtschenok`. Паспортным алфавитом вышло бы `Privet, zheltyi shchenok`, ISO 9 — `Privet, žëltyj ŝenok`.
