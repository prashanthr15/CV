```mermaid
graph TD
  A[Start] --> B{Is user registered?}
  B -- No --> C[Register]
  B -- Yes --> D[Login]
  D --> E[Choose Role]
  ...
