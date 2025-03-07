# Проектная работа "Веб-ларек"

Стек: HTML, SCSS, TS, Webpack

Структура проекта:
- src/ — исходные файлы проекта
- src/components/ — папка с JS компонентами
- src/components/base/ — папка с базовым кодом

Важные файлы:
- src/pages/index.html — HTML-файл главной страницы
- src/types/index.ts — файл с типами
- src/index.ts — точка входа приложения
- src/scss/styles.scss — корневой файл стилей
- src/utils/constants.ts — файл с константами
- src/utils/utils.ts — файл с утилитами


## Установка и запуск
Для установки и запуска проекта необходимо выполнить команды

```
npm install
npm run start
```

или

```
yarn
yarn start
```
## Сборка

```
npm run build
```

или

```
yarn build
```


## Описание базовых классов

### Класс `Api`.

Методы:
- `constructor` - конструктор класса.
- `handleResponse` - обработчик ответа сервера.
- `get` - принимает изменяющеюся часть url-адреса, возвращает ответ от сервера.
- `post` - принимает изменяющеюся часть url-адреса, принимает данные в виде объекта для отправки на сервер.

### Класс `EventEmitter`, implements `IEvents`.

Методы:
- `constructor` - конструктор класса.
- `on` - для подписки на событие.
- `off` - для отписки от события.
- `emit` - уведомления подписчиков о наступлении события соответственно.
- `onAll` - для подписки на все события.
- `offAll` - сброса всех подписчиков.
- `trigger` - генерирует заданное событие с заданными аргументами. 

## Используемые паттерны проектирования

* Observer — класс `EventEmitter` управляет подписчиками и уведомляет их при возникновении события.
* Factory Method — функция `createElement` создает DOM-элемент заданного типа, устанавливает свойства и добавляет вложенные элементы.


<!--## UML-схема-->

