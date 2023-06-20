```mermaid
stateDiagram-v2
  direction LR
  [*] --> Backlog
  Backlog --> addBugs
  addBugs --> findBugs
  findBugs --> Backlog
  addBugs --> runOutOfTime
  runOutOfTime --> releaseAnyway
  releaseAnyway --> findMoreBugs
  findMoreBugs --> Backlog
```
