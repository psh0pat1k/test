# Chat log — Diagram 4 (Class diagram)

**Prompt:**

```
Представь, что ты системный архитектор. Напиши код для Mermaid classDiagram, описывающий простую клиентскую библиотеку API с классами APIClient, Auth, and Cache. Добавь заметку или подпись 'Author: egor_shalin'.
```

**LLM response (пример):**

```mermaid
classDiagram
    class APIClient {
        +get(endpoint)
        +post(endpoint, data)
    }
    class Auth {
        +login(credentials)
        +refresh()
    }
    class Cache {
        +get(key)
        +set(key, value)
    }

    APIClient --> Auth : uses
    APIClient --> Cache : caches

    note right of APIClient: Author: egor_shalin
```

Скопируйте код в `artifacts/diagram_4_code.md` и экспортируйте PNG.
