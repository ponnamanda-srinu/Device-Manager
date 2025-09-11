flowchart TD
  A[Click Generate button] --> B[Enter login password]
  B --> C[Generate invoice record]
  C --> D[Click Refresh button]
  D --> E{Network available?}
  E -- Yes --> F[Sync to server green]
  E -- No  --> G[Queued for sync offline]
  F --> H[Summary]
  F --> I[Manage]
  F --> J[Authorize]
  F --> K[Delete]
  G --> H
  G --> I
  G --> J
  G --> K

