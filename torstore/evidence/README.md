# Evidence по тестированию Tor Store

Папка предназначена для обезличенных доказательств, связанных с отчётом по тестированию Tor Store.

## Типы evidence

Можно добавлять:

- screenshots воспроизведённых дефектов;
- screenshots Chrome DevTools Network;
- screenshots Console / Issues;
- screenshots responsive layout;
- обрезанные сравнения сайта с design requirements;
- обезличенные response fragments;
- короткие screen recordings.

## Рекомендуемые названия

- `TS-BUG-001-header-mockup-mismatch.png`
- `TS-BUG-002-javascript-resource-404.png`
- `TS-BUG-003-search-result-counter.png`
- `TS-BUG-004-social-links-navigation.png`
- `TS-BUG-005-csp-issue.png`
- `TS-BUG-006-form-label-accessibility.png`
- `TS-BUG-007-main-page-mockup-mismatch.png`

## Безопасность перед публикацией

Evidence необходимо проверить на отсутствие:

- email и passwords;
- session cookies;
- authentication tokens;
- API keys;
- персональных данных;
- browser history и посторонних tabs;
- private URLs;
- request headers с authorization data;
- конфиденциальных материалов компании или курса.

## Правила репозитория

- Raw HAR не публикуются, так как могут содержать cookies и authorization data.
- Крупные видео хранятся отдельно.
- Screenshots обрезаются до релевантной области.
- Sensitive values скрываются или заменяются placeholders.
- Каждый evidence item должен ссылаться на соответствующий Bug ID.
- Design materials не публикуются без разрешения.

## Текущий статус

Ссылки на evidence зафиксированы в Excel-отчёте.

Дополнительные screenshots добавляются только после проверки содержимого, релевантности и безопасности публикации.
