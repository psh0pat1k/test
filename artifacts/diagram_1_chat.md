# Chat log — Diagram 1 (Sequence)

**Prompt:**

```
Представь, что ты системный архитектор. Напиши код для Mermaid sequence диаграммы, которая описывает процесс авторизации пользователя через OAuth (клиент → браузер → авторизационный сервер → бэкенд). Обязательно добавь на схему блок или подпись 'Author: egor_shalin'.
```

**LLM response (пример):**

```mermaid
sequenceDiagram
    participant User as User["egor_shalin"]
    participant Browser as Browser
    participant Auth as AuthServer
    participant Backend as Backend

    User->>Browser: Открывает страницу входа
    Browser->>Auth: Перенаправление на OAuth (запрос авторизации)
    Auth-->>Browser: Redirect с кодом авторизации
    Browser->>Backend: Отправка кода на бэкенд
    Backend->>Auth: Обмен кода на access_token
    Auth-->>Backend: access_token
    Backend-->>Browser: Создание сессии / cookie
    Browser-->>User: Авторизация успешна

    Note over User,Backend: Author: egor_shalin
```

Скопируйте блок кода из ответа в `artifacts/diagram_1_code.md` и вставьте в Mermaid Live Editor для экспорта PNG.
