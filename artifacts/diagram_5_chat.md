# Chat log — Diagram 5 (Gantt)

**Prompt:**

```
Представь, что ты системный архитектор/проектный менеджер. Напиши код для Mermaid Gantt диаграммы, описывающей простой 3-недельный план: дизайн, разработка, тестирование. В заголовке укажи 'Author: egor_shalin'.
```

**LLM response (пример):**

```mermaid
gantt
    title Project Timeline — Author: egor_shalin
    dateFormat  YYYY-MM-DD
    section Sprint 1
    Design       :des1, 2025-12-01, 7d
    Develop      :dev1, after des1, 14d
    Test         :test1, after dev1, 7d
```

Скопируйте код в `artifacts/diagram_5_code.md` и экспортируйте PNG.
