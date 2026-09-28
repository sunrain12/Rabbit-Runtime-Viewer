# Rabbit-Runtime-Viewer— MVP 0.1
# 🐇 Rabbit Runtime Viewer — MVP 0.1

> An interactive AI-powered runtime viewer with two rabbit characters.

Rabbit Runtime Viewer is an experimental interactive web experience that visualizes my computer activity through an AI interface.

Two rabbit characters observe the runtime data and interact with me through conversation.

## ✨ Concept

```text
                    ┌──────────────────┐
                    │   RunTime Tracker │
                    │   Activity Data   │
                    └────────┬─────────┘
                             │
                             ▼
┌──────────────┐      ┌──────────────┐      ┌──────────────┐
│   🐰 Rabbit A │ ◄──► │   Backend    │ ◄──► │   DeepSeek   │
└──────────────┘      └──────┬───────┘      └──────────────┘
                             │
                             ▼
                      ┌──────────────┐
                      │ Runtime View │
                      └──────────────┘
                             ▲
                             │
┌──────────────┐             │
│   🐰 Rabbit B │ ───────────┘
└──────────────┘
```

## 🎯 MVP 0.1

The first version focuses on four things:

* [ ] Display runtime/activity data
* [ ] Show two interactive rabbit characters
* [ ] Chat with Rabbit A
* [ ] Chat with Rabbit B
* [ ] Allow rabbits to react to runtime data

## 🧠 AI

The project uses the DeepSeek API as the language model backend.

Each rabbit has its own:

* personality
* system prompt
* conversation history
* behavior

The two rabbits initially share the same runtime data source.

## ⏱️ Runtime Data

Runtime information is provided by:

**RunTime_Tracker**

https://github.com/1812z/RunTime_Tracker

RunTime_Tracker provides the underlying activity tracking and data storage.

Rabbit Runtime Viewer acts as an interactive visualization and AI layer on top of it.

## 🏗️ Architecture

```text
Browser
   │
   ▼
Frontend (Vue)
   │
   ▼
Backend (Node.js)
   │
   ├──────────────► DeepSeek API
   │
   └──────────────► RunTime_Tracker API
```

The DeepSeek API key is kept on the backend and is never exposed to the browser.

## 🚧 Development Status

### MVP 0.1

Currently under development.

The initial goal is to build the basic interactive experience before introducing more advanced agent behavior.

Future versions may include:

* autonomous rabbit behavior
* long-term memory
* rabbit-to-rabbit conversations
* event-driven reactions
* tool calling
* agent harness integration

## 📜 License

MIT
