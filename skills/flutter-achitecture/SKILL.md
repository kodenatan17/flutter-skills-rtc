---
name: flutter-architecture
description: Enforce clean architecture principles in Flutter features, ensuring proper layering, separation of concerns, and maintainable code structure.
metadata:
  model: models/gemini-3.1-pro-preview
  last_modified: Sat, 2 May 2026 19:45:59 GMT
---

## Inject Rules

* Use Clean Architecture:
  UI → Bloc → UseCase → Repository → Data

* Enforce SSOT:

  * State only in Bloc
  * No duplicated state

* WebRTC must be wrapped:

  * No direct usage in Bloc/UI
  * Use Data layer wrapper

* Dependency rule:

  * Bloc depends on UseCase
  * UseCase depends on abstraction
