# Groupz - Real-Time AI Chat Ecosystem

![Groupz Header](https://res.cloudinary.com/dlb65j6di/image/upload/v1721924193/groupz_header.png)

Groupz is a sophisticated real-time communication platform built with Django. It bridges the gap between traditional messaging and modern AI, allowing users to interact with advanced Large Language Models (LLMs) directly within their group conversations.

## Features

*   **User Authentication**: Secure registration and login system for a personalized experience.
*   **Private & Group Messaging**: Seamless direct chats and robust group management features.
*   **AI Integration**: Mention `@gemini` or `@llama3` in any group chat to trigger real-time AI responses powered by the Groq inference engine.
*   **Real-time Synchronization**: Utilizing WebSockets for instantaneous message delivery and status updates.
*   **Admin Controls**: Group creators can manage memberships and moderate threads effectively.

## Technical Architecture

The platform is designed for high concurrency and low latency, utilizing an asynchronous backend stack.

![Groupz UI Interface](https://res.cloudinary.com/dlb65j6di/image/upload/v1721924193/groupz_ui.png)

### Backend & AI Logic
*   **Framework**: Python & Django (utilizing Channels and ASGI for asynchronous support).
*   **Inference**: Groq (Llama3 8B) and Google Generative AI for intelligent group interactions.
*   **State Management**: Redis serves as the backing store for WebSockets and caching.

### Infrastructure
*   **Database**: PostgreSQL for persistent user and message data.
*   **Deployment**: Hosted on Render using a containerized environment to ensure scalability.

## Development Stack

*   **Languages**: Python, JavaScript
*   **Backend**: Django, Channels, Daphne, Redis
*   **Frontend**: HTML5, CSS3, Bootstrap 5
*   **AI**: LangChain, Groq API, Google Gemini API

## Repository

The full source code and deployment instructions are available on GitHub:
[GitHub - Groupz Chat App](https://github.com/kasun98/Groupz)

---
© 2025 | Groupz - AI Integrated Messaging
