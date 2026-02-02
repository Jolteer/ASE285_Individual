# System Architecture

## Overview

```
┌─────────────────────────────────────────────────────────────┐
│                    Electron Application                      │
│  ┌────────────────────────────────────────────────────────┐ │
│  │                    React Frontend                       │ │
│  │  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐  │ │
│  │  │   App.jsx    │  │  Dashboard   │  │   Sidebar    │  │ │
│  │  └──────────────┘  └──────────────┘  └──────────────┘  │ │
│  │                          │                              │ │
│  │                    ┌─────▼─────┐                        │ │
│  │                    │   Chat    │                        │ │
│  │                    └───────────┘                        │ │
│  └────────────────────────────────────────────────────────┘ │
│                              │                               │
│  ┌───────────────────────────▼────────────────────────────┐ │
│  │                   Redux Store                           │ │
│  │              (dashboardSlice.js)                        │ │
│  └─────────────────────────────────────────────────────────┘ │
│                              │                               │
│  ┌───────────────────────────▼────────────────────────────┐ │
│  │               OpenAI Service                            │ │
│  │            (openaiService.js)                           │ │
│  └─────────────────────────────────────────────────────────┘ │
└─────────────────────────────────────────────────────────────┘
                               │
                               ▼
                    ┌─────────────────┐
                    │   OpenAI API    │
                    │   (External)    │
                    └─────────────────┘
```

## Components

### Frontend (React)

- **App.jsx**: Main application component, initializes OpenAI and loads conversations
- **Dashboard.jsx**: Main layout component with sidebar and chat area
- **Chat/**: Components for displaying and sending messages
- **Sidebar/**: Components for conversation list and navigation

### State Management (Redux)

- **store.js**: Redux store configuration
- **dashboardSlice.js**: Redux slice containing:
  - Conversation state
  - Message handling
  - Async thunks for AI communication

### Services

- **openaiService.js**: Handles all OpenAI API communication
  - Initialize API client
  - Send messages to AI
  - Handle responses

### Desktop (Electron)

- **main.js**: Electron main process
- **preload.js**: Preload script for secure IPC

### Storage

- **localStorage**: Persists conversations and settings locally

## Technology Stack

- **React 18**: UI framework
- **Redux Toolkit**: State management
- **Vite**: Build tool and dev server
- **Electron**: Desktop application wrapper
- **OpenAI SDK**: AI integration
