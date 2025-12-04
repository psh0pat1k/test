```mermaid
erDiagram
    USER {
        int id
        string nickname
    }
    POST {
        int id
        string title
        string body
    }
    COMMENT {
        int id
        string body
    }

    USER ||--o{ POST : writes
    POST ||--o{ COMMENT : has

    %% Author: egor_shalin
```
