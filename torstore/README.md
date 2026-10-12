# Тестирование веб-приложения Tor Store

Независимый практический проект по ручному black-box тестированию и test design веб-приложения **Tor Store**.

Проект включает functional testing, документированный smoke-прогон, сравнение UI с макетом, negative test design, начальные responsive checks и технический анализ через Chrome DevTools.

## Объект тестирования

| Параметр | Значение |
|---|---|
| Приложение | Tor Store |
| Платформа | Web |
| Окружение | Public test environment |
| URL | `ts.red-promo.ru` |
| Отчёт обновлён | 2026-05-19 |
| Подход | Ручное black-box testing |
| Браузер | Google Chrome |
| OS | Не зафиксирована |
| Язык исходного отчёта | Английский |

## Область тестирования

Документация покрывает:

- главную страницу и header;
- navigation и catalog;
- product cards;
- Favorites;
- cart и quantity controls;
- checkout test design;
- Search;
- callback и authentication forms;
- Contacts и footer;
- сравнение UI с design mockup;
- negative scenarios;
- начальные responsive checks;
- Chrome DevTools Network / Console / Issues;
- accessibility observations.

Часть negative, cart, checkout и responsive scenarios была спроектирована, но не выполнена полностью. Такие проверки оставлены со статусами `Not Run` или `In Progress`.

## Тестовая документация

| Артефакт | Количество |
|---|---:|
| Smoke test cases | 22 |
| Functional test cases | 51 |
| Functional checklist items | 34 |
| UI / mockup checks | 10 |
| Negative test scenarios | 11 |
| Баг-репорты | 7 |

## Результаты smoke-прогона

| Статус | Количество |
|---|---:|
| Passed | 4 |
| Failed | 5 |
| In Progress | 1 |
| Not Run | 12 |

Статус `Passed` используется только для фактически выполненных проверок. Невыполненные и незавершённые сценарии отмечены отдельно.

## Основные дефекты

### Functional / navigation

- `BUG-003` — Search показывает некорректное количество товаров и противоречивое сообщение об отсутствии результатов.
- `BUG-004` — иконки социальных сетей ведут на страницу Contacts вместо соответствующих внешних сервисов.

### Technical

- `BUG-002` — обязательный JavaScript resource `select22.min.js` возвращает `404 Not Found`.
- `BUG-005` — Content Security Policy блокирует JavaScript string evaluation.
- `BUG-006` — form controls некорректно связаны с labels.

### UI / design

- `BUG-001` — пункты header menu и номер телефона не соответствуют предоставленному design mockup.
- `BUG-007` — блоки главной страницы, banners, contact information и footer частично отличаются от макета.

## Трассировка

В отчёте связаны:

- функциональные области;
- functional test cases;
- smoke scenarios;
- Bug IDs;
- execution statuses;
- QA review comments.

Это позволяет разделять подтверждённые результаты, failed behaviour, незавершённые проверки, UI mismatches и technical findings.

## Инструменты и техники

- Google Chrome;
- Chrome DevTools Network;
- Chrome DevTools Console / Issues;
- ручное functional testing;
- test cases и checklists;
- positive / negative testing;
- initial responsive testing;
- сравнение с design mockup;
- bug reporting;
- Severity / Priority assessment;
- traceability matrix.

## Артефакты

- [Tor Store Web Testing Report](artifacts/torstore-web-testing-report.xlsx)
- [Правила публикации evidence](evidence/README.md)

## Ограничения

- полный functional suite не выполнен;
- cart и checkout требуют дополнительного контролируемого прогона;
- responsive testing не завершён для всех целевых ширин;
- полная browser / OS compatibility matrix не проверялась;
- source code и server-side implementation недоступны;
- формальные требования были ограничены;
- часть UI validation выполнялась по предоставленному макету;
- тестируемый сайт может измениться после зафиксированного прогона;
- design PDF в репозитории не распространяется.

## Дисклеймер

Это независимый практический QA portfolio project.

Тестируемый сайт, visual materials, product names и trademarks принадлежат соответствующим владельцам. Репозиторий не содержит proprietary source code или confidential materials.
