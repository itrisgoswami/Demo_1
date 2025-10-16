# Momentum AI
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Technology-Stack](https://img.shields.io/badge/Stack-HTML%2FCSS%2FJS-orange)](https://developer.mozilla.org/en-US/docs/Web)
[![AI-Powered](https://img.shields.io/badge/Powered%20By-Google%20Gemini-4285F4)](https://ai.google.dev/gemini-api)

## Description

Momentum AI is an innovative, client-side web application designed to empower users in establishing and maintaining habits while providing personalized, AI-driven guidance for achieving broader life goals. It uniquely combines a robust, smart habit tracker with an integrated AI planning assistant, operating seamlessly within the browser for speed and accessibility.

Built using standard web technologies (HTML, CSS, JavaScript), the project emphasizes a dynamic user experience and powerful real-time data persistence. What sets Momentum AI apart is its **AI Guidance Module**, which leverages the Google Gemini AI (via its JavaScript SDK) to transform complex objectives into manageable, actionable steps, serving as a personal coach right in the browser.

## Features

*   **Smart Habit Tracker:** Core features include daily check-ins, visual streak maintenance, and flexible habit definitions.
*   **Visual Progress Indicators:** Engaging feedback, such as a visually growing plant or escalating streak counters, motivates users to maintain consistency.
*   **Persistent Client-Side Storage:** All user data (habits, streaks, progress) is securely stored in the browser's `localStorage`, ensuring data persists across sessions without the need for a backend server or login.
*   **Integrated AI Guidance:** Direct integration with the **Google Gemini AI** allows for dynamic generation of structured action plans.
*   **Personalized Goal Planning:** Users can define any life goal, and the AI generates intelligent, step-by-step roadmaps, breaking down complex tasks into easily digestible and actionable steps.
*   **Client-Side Architecture:** Designed for rapid deployment and maximum accessibility, running entirely within the user's web browser.

## Technology Stack

Momentum AI is a purely client-side application utilizing modern web standards:

| Component | Technology | Role |
| :--- | :--- | :--- |
| **Structure** | `HTML5` | Defines the application interface and structure. |
| **Styling** | `CSS3` | Provides dynamic styling, responsiveness, and visual engagement. |
| **Logic** | `JavaScript (ES6+)` | Handles application state, DOM manipulation, data persistence, and AI API calls. |
| **AI Integration** | `Google Gemini AI SDK (JavaScript)` | Powers the goal planning and coaching features. |

## Installation

As Momentum AI is a client-side application, setup is quick and requires no compilation or complex dependencies.

1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/your-username/momentum-ai.git
    cd momentum-ai
    ```
2.  **Open in Code Editor:**
    Paste the codes (or open the cloned directory) into your preferred code editor (e.g., VS Code).
3.  **Launch the Application:**
    Simply open the `index.html` file directly in your web browser. *(Note: For a more robust local development experience, it is recommended to use a simple local server extension like VS Code's Live Server.)*

## Configuration (Crucial Step for AI)

To enable the powerful AI Guidance Module, you must provide your Google Gemini API key within the project's JavaScript code.

1.  **Obtain API Key:** Acquire a key from Google AI Studio.
2.  **Configure Key:** Locate the relevant JavaScript file where the Gemini SDK is initialized (e.g., `scripts/ai_guidance.js`). Replace the placeholder text with your actual API key.

```javascript
// Example of where to place the key (may vary based on project structure)
const API_KEY = "YOUR_GEMINI_API_KEY_HERE";
// ... Initialize the model with the key
```

> **Security Warning:** Since this is a purely client-side application, the API key is exposed in the front-end code. This architecture is suitable for prototypes, hackathons, or personal use. For public deployment or production environments, a secure backend proxy is strongly recommended to protect your credentials.

## Usage

Momentum AI is intuitive, separating core habit management from AI-powered future planning.

### 1. Habit Tracking

1.  **Define a New Habit:** Input the name of the habit you wish to track (e.g., "Read 30 minutes," or "Meditate").
2.  **Daily Check-in:** On the main dashboard, click the checkbox or indicator corresponding to the day to register completion.
3.  **Maintain Streaks:** Observe the visual progress indicators to track your consistency. Data is automatically saved to your browser.

### 2. AI Goal Guidance

1.  **Input Your Goal:** Navigate to the AI Guidance section and define a complex, long-term objective (e.g., "Run a marathon in six months," or "Build a basic e-commerce website").
2.  **Request Guidance:** Click the button to send the goal to the Gemini AI.
3.  **Review Action Plan:** The application will display a clear, structured action plan, often broken down week-by-week or phase-by-phase, providing concrete steps to achieve your defined goal.

## Contributing

We welcome community involvement and contributions to Momentum AI. While built rapidly, the project offers significant opportunities for expansion, feature additions, and refining the AI interaction models.

We appreciate all appropriate pull requests and will review them promptly.

**How to Contribute:**

1.  **Fork the Repository:** Start by forking the project to your own GitHub account.
2.  **Create a Feature Branch:** Create a new branch for your specific changes, using a descriptive name (e.g., `feat/add-settings-menu`, `fix/mobile-layout-bug`).
    ```bash
    git checkout -b your-feature-branch
    ```
3.  **Implement Changes:** Make your necessary modifications and ensure the code adheres to existing style guidelines.
4.  **Commit and Push:** Commit your changes with clear, concise messages.
5.  **Generate Appropriate Pull Requests:** Submit a Pull Request (PR) against the `main` branch of the original repository. Please ensure your PR description clearly explains the problem solved or the feature added.

We will see and respond to all appropriate pull requests efficiently.

## License

Distributed under the MIT License. See the `LICENSE` file for more information.
