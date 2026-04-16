# EduTrack Pro

EduTrack Pro is a production-style frontend web application for the **Education / Training Platform** domain. It was designed to satisfy the Assignment 2 brief for ICT930 by demonstrating modern frontend architecture, reusable React components, async data handling, responsive UI/UX, accessibility, and maintainable code.

## Project Overview

The application allows users to:
- discover and filter training courses
- complete an enrolment form with validation
- track enrolled courses in a shared dashboard
- visualise progress through lesson completion and summary analytics
- submit support requests through an accessible form

## Technology Stack

- **React 18** with functional components and hooks
- **Vite** for development and build tooling
- **React Router DOM** for client-side routing
- **Context API + useReducer** for shared application state
- **ESLint** for code quality
- **CSS** for responsive layout and design system styling
- **Mock JSON data** with asynchronous service wrappers

## Key Features

### 1. Multi-page navigation
- Home
- Courses
- My Learning
- Support
- 404 Not Found

### 2. Reusable component architecture
- shared layout components
- reusable feedback states
- reusable cards, filters, modal, stats, and progress components

### 3. State management
- local state for forms, filters, accordion, and modal behaviour
- shared state using Context API + useReducer for enrolments, toast feedback, and support requests
- persistence using localStorage for a better user experience

### 4. Data handling
- mock JSON course catalogue
- asynchronous loading through `courseService.js`
- explicit loading, error, and empty states

### 5. User interaction
- course search and filtering
- enrolment modal with client-side validation
- lesson completion toggles with live progress updates
- reminder preference toggles
- support form validation
- FAQ accordion interaction

### 6. Responsive and accessible design
- mobile and desktop layouts
- semantic HTML structure
- labelled forms
- keyboard-accessible buttons and controls
- skip link
- aria-live feedback for toast messages and loading states
- clear spacing, visual hierarchy, and contrast

## Folder Structure

```text
src/
  components/
  context/
  data/
  pages/
  services/
  styles/
  utils/
```

## Installation Instructions

1. Open a terminal in the project folder.
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm run dev
   ```
4. Open the local URL shown in the terminal.

## Build for Production

```bash
npm run build
```

## Linting

```bash
npm run lint
```

## Design Decisions

- **React + Vite** was selected because it is the simplest high-productivity option from the brief while still aligning with current industry practice.
- **Education / Training Platform** was chosen because it naturally supports all mandatory features in a cohesive way: discovery, enrolment, progress tracking, forms, and dashboards.
- **Context API** was sufficient for the scale of this assignment and avoided unnecessary complexity from external state libraries.
- **Mock async services** were used to simulate real frontend behaviour while keeping the project fully self-contained.
- **Query parameters** were used on the Courses page to preserve filter state and support direct navigation to modal states.

## Screenshots Included

The `screenshots/` folder contains desktop and mobile captures for:
- Home page
- Courses page
- Enrolment modal
- My Learning dashboard
- Support page
- Mobile course view

## Assessment Alignment Summary

This project directly addresses the brief by including:
- client-side routing
- reusable component architecture
- local and shared state
- async data handling with loading and error states
- validated forms and dynamic interactions
- responsive design
- accessibility considerations
- README and reflection documentation

## Notes for Submission

- Update the reflection in your own voice if your institution requires personal commentary.
- If AI tools were used during development, disclose that use exactly as required by your course policy.
