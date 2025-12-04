```mermaid
graph LR
    subgraph "Author: @egor_shalin"
    end
    Start[Start] --> Plan[Plan]
    Plan --> Dev[Develop]
    Dev --> Test[Test]
    Test --> |OK| Release[Release]
    Test --> |Fail| Dev
    Release --> Monitor[Monitor]
    Monitor --> Plan
```
