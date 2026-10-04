# Drive Exchange Inbox Bridge

STATUS: ACTIVE EXPERIMENTAL BRIDGE  
SCOPE: COMPANY-WIDE  
TASK: GME-DRIVE-INBOX-007

## Purpose

Provide a return path for authorized AI workers that can read the Public Memory Exchange but cannot write GitHub directly.

This bridge is NON-CANONICAL. It does not change the authority model.

## Entry

Google Doc: GuluAI AI Exchange Inbox — START HERE

https://docs.google.com/document/d/1p2jJRKaZYQNtIJLoVnp7KDu2zvoE3GXt0ECOl9oqq14/edit

Drive folder: GuluAI AI Exchange Inbox

https://drive.google.com/drive/folders/1O8Tpi3H02mEDP8tUxg3Mbs4WTBoruXkV

## Route

Public START-HERE
→ assigned handoff
→ authorized work
→ if direct Public Exchange write is unavailable, use Drive Exchange Inbox
→ authorized reconciler verifies result
→ public-safe result/receipt enters Public Exchange
→ canonical reconciliation where required

## Rules

- Public Exchange remains NON-CANONICAL.
- Drive Inbox is also NON-CANONICAL.
- Private GitHub canonical systems remain authoritative after reconciliation.
- Never place secrets, credentials, student PII, sensitive contracts/finance, private repo content, or other non-public-safe material into a result intended for the Public Exchange.
- Human should not transport detailed reports between agents.
- A worker using this bridge should return only a short completion acknowledgement to the Human.
- Folder-level sharing is not assumed by this protocol. Access must be tested by the worker. The START HERE document is verified shared Writer with both GuluAI core accounts.
