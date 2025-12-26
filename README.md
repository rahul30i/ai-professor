# AI Professor 🎓

> **A Next-Generation Educational Interface powered by Generative AI.**

The **AI Professor** is a sophisticated React application designed to simulate a one-on-one tutoring session with a distinguished academic. Unlike standard chatbots, the AI Professor utilizes domain-specific prompting and structured data streaming to deliver lectures that are not only informative but also visually engaging.

## 🏗 Architecture & Design

This project follows a **Principal Engineer** standard, prioritizing:
-   **Defensive Coding**: graceful degradation when API limits are reached.
-   **Domain-Driven Design (DDD)**: Code variables reflect the "Academic" domain (`lectureContent`, `studentQuery`) rather than generic CRUD terms.
-   **Type Safety**: Full TypeScript implementation with strict interfaces for JSON streams.

### Core Architecture
-   **Frontend**: React + Vite (Fast HMR, optimized bundling).
-   **AI Layer**: Google Gemini API (via `@google/genai` SDK).
-   **State Management**: React Hooks with streaming buffers.
-   **Visuals**: Smart YouTube Search embedding based on AI-generated queries.

## 🚀 Getting Started

### Prerequisites
-   Node.js v18+
-   A valid [Google Gemini API Key](https://aistudio.google.com/app/apikey)

### Installation

1.  **Clone the department archives**:
    ```bash
    git clone https://github.com/your-username/ai-professor.git
    cd ai-professor
    ```

2.  **Install dependencies**:
    ```bash
    npm install
    ```

3.  **Configure Environment**:
    Create a `.env` file in the root directory:
    ```env
    VITE_API_KEY=your_gemini_api_key_here
    ```

4.  **Launch the Campus**:
    ```bash
    npm run dev
    ```
    Open `http://localhost:5173` to attend class.

## 📚 Project Structure

```
ai-professor/
├── src/
│   ├── components/      # UI Components (Avatar, Input, Display)
│   ├── services/        # AI Service Layer (Gemini Integration)
│   ├── App.tsx          # Main Lecture Hall Logic
│   └── main.tsx         # Entry Point
├── package.json         # Dependency Manifest
└── vite.config.ts       # Build Configuration
```

## 🛡 Disclaimer

*The AI Professor is an experimental educational tool. While highly knowledgeable, the Professor may occasionally hallucinate facts or visual aids. Always verify citations with primary sources.*
