# ⏱️ React Stopwatch

A responsive and accurate **stopwatch** built with **React.js**, featuring real-time millisecond updates. It supports **Start**, **Stop**, and **Reset** functionalities using React Hooks and `useRef`.

## 🚀 Features

- Start, Stop, and Reset buttons
- Displays minutes, seconds, and milliseconds
- Updates every 10 milliseconds
- Uses `useState`, `useEffect`, and `useRef` for precise control
- Functional component architecture

## 🧠 How It Works

- `useState` manages the stopwatch state (`isRunning`, `elapsedTime`)
- `useRef` stores interval and time references without triggering re-renders
- `setInterval` runs every 10ms to update the time while running
- Cleanup via `clearInterval` prevents memory leaks on unmount or stop

## 📦 Usage

1. Copy the `Stopwatch.js` file into your React project.
2. Import and use the component:

```jsx
import React from 'react';
import Stopwatch from './Stopwatch';

function App() {
  return (
    <div>
      <h1>Stopwatch</h1>
      <Stopwatch />
    </div>
  );
}

export default App;
