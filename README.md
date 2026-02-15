# Frontend Second Semester Examination Project - Todo App

A robust, accessible, and responsive Todo application built with React, TypeScript, Tailwind CSS, and ShadCN/UI.

## Features

- **Todo Management**: View, search (client-side), and filter todos with pagination.
- **Bonus Features**:
    - **Create & Delete**: Add new tasks via a modal and remove them (optimistic UI updates).
- **Detailed View**: Dedicated page for individual todo details.
- **Responsive Design**: Mobile-first approach ensuring usability across all devices.
- **Accessibility**: Semantic HTML, ARIA attributes, and keyboard navigation support.
- **Error Handling**: Global Error Boundary, Toast notifications, and custom 404 pages.
- **Theme Support**: Dark/Light mode toggle.

## Tech Stack

- **Framework**: React 19+ (Vite)
- **Language**: TypeScript
- **Styling**: Tailwind CSS v3
- **UI Components**: ShadCN/UI (Manual implementation: Card, Button, Input, Dialog, Badge)
- **Routing**: React Router DOM v7
- **State Management/API**: Tanstack Query (React Query) & Axios
- **Icons**: Lucide React

## Setup Instructions

1.  **Clone the repository:**
    ```bash
    git clone <repository-url>
    cd todo-app
    ```

2.  **Install dependencies:**
    ```bash
    npm install
    ```

3.  **Start development server:**
    ```bash
    npm run dev
    ```
    Open [http://localhost:5173](http://localhost:5173) in your browser.

4.  **Build for production:**
    ```bash
    npm run build
    ```
    The build output will be in the `dist` directory.

## Known Issues & Notes

> **Important:** The backend API (`https://api.oluwasetemi.dev/todos`) is currently returning `404 Not Found` or failing to connect.
> 
> **Robust Error Handling Features:**
> 1.  **Detection**: The app identifies the API failure immediately.
> 2.  **Notification**: A toast notification alerts the user: *"API Unreachable: Switched to Demo Mode"*.
> 3.  **Resilience**: Instead of crashing or showing a blank screen, the app seamlessly switches to **Mock Data Mode**.
> 4.  **Functionality**: Users can still **Create, Read, and Delete** tasks, demonstrating that the frontend logic remains solid even when external dependencies fail.

## Future Improvements

- **Authentication**: Full login/registration flow (Request/Response interfaces are typed).
- **Real-time Updates**: WebSocket integration for collaborative lists.
- **Persistent Storage**: LocalStorage backup for offline capability.

---
Submitted by: [Your Name]
