# 📌 Chatbot Web App – Detailed Description
https://pixyz-bit.github.io/SSDev-Chatbot/
## 1. Overview: What This Program Does

This project is a **single-page chatbot web application built with React**. It provides an interactive chat interface where users can communicate with a chatbot in real time.

The application allows users to:

- Type messages into an input box  
- Send messages by clicking **Send** or pressing **Enter**  
- View messages in a chat-style interface  
  - User messages appear on the **right**
  - Bot messages appear on the **left**
- See a **loading spinner** while waiting for the chatbot’s response  
- Automatically scroll the chat window to display the **latest message**

---

## 2. Technologies and Concepts Used

The application is built using modern React concepts and web technologies:

- **React functional components**
- **React Hooks**
  - `useState` for state management
  - `useRef` for direct DOM access
  - `useEffect` for handling side effects
- **Custom React Hook** for automatic scrolling
- **External Chatbot API**
  - `Chatbot.getResponseAsync` for generating bot replies
- **HTML & CSS** for layout and styling

---

## 3. High-Level Structure

The project is organized into three main layers:

### 1. Presentation Layer
- HTML structure for mounting the React app
- CSS styles for layout, chat bubbles, buttons, and scrolling behavior

### 2. Component Layer (React UI)
- Modular React components for better separation of concerns

### 3. Logic Layer
- State management
- Asynchronous message handling
- Auto-scroll functionality

---

## 4. Main React Components

### `App` (Root Component)
- Serves as the main entry point of the application
- Manages the global chat messages state
- Passes data and handlers down to child components

### `ChatMessages`
- Renders the list of chat messages
- Uses a custom hook to automatically scroll when messages update

### `ChatMessage`
- Displays a single chat message
- Adjusts layout based on sender (user or bot)
- Shows profile images accordingly

### `ChatInput`
- Handles user text input
- Sends messages to the chatbot
- Displays loading state during API calls

### `useAutoScroll` (Custom Hook)
- Automatically scrolls the chat container to the newest message
- Uses `useRef` and `useEffect` to interact with the DOM safely

---

## 5. User Experience Flow

1. The application loads and displays a welcome message.
2. The user types a message into the input box.
3. The message is sent via button click or Enter key.
4. The message appears instantly in the chat window.
5. A loading spinner is shown while waiting for the bot’s reply.
6. The chatbot response replaces the loading indicator.
7. The chat window automatically scrolls to the bottom.

---

## 6. Summary

This chatbot application demonstrates:

- Effective use of React hooks
- Separation of UI, logic, and state
- Handling asynchronous operations cleanly
- Implementing DOM interactions safely using refs
- Providing a smooth and intuitive chat experience

It is an excellent example of a beginner-to-intermediate React project that applies real-world concepts in a practical way.

---

✅ **Ready to use as a GitHub README.md**
