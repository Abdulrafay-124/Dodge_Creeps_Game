flowchart TD
  A[Home] --> B[Shop]
  B --> C[Checkout]
  C --> D{Form Valid?}
  D -->|No| E[Show Errors]
  D -->|Yes| F[Simulate Payment]
  F --> G{Result}
  G -->|Success| H[Order Confirmed]
  G -->|Declined| I[Payment Declined]
  G -->|Network| J[Try Again]
