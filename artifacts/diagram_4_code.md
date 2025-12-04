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
