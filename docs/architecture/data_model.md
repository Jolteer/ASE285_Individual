# Data Model

## Entity Relationship Diagram

```
┌─────────────────────┐         ┌─────────────────────┐
│    Conversation     │         │      Message        │
├─────────────────────┤         ├─────────────────────┤
│ - id: string        │ 1     * │ - id: string        │
│ - title: string     │─────────│ - content: string   │
│ - createdAt: date   │         │ - role: string      │
│                     │         │ - timestamp: date   │
└─────────────────────┘         └─────────────────────┘
```

## Entities

### Conversation

- **id**: Unique identifier (UUID)
- **title**: Conversation title (auto-generated or user-defined)
- **createdAt**: Timestamp when conversation was created
- **messages**: Array of Message objects

### Message

- **id**: Unique identifier (UUID)
- **content**: Message text content
- **role**: Either 'user' or 'assistant'
- **aiMessage**: Boolean flag indicating if message is from AI
- **timestamp**: When the message was sent

## Relationships

- A **Conversation** has many **Messages** (1:N relationship)
- Messages are stored in order within a conversation
- Conversations are persisted to localStorage
