# Newsify

Newsify is a mobile-first news application built with React and the New York Times API. Users can browse stories by category, customize their feed, swipe through articles and save stories to a personal archive.

[View the live application](https://reeds-newsify.netlify.app/)

This project was developed during my Web Developer education and is included in my portfolio because it demonstrates more than a simple API fetch: it combines reusable data-fetching logic, shared state, persistence, routing, testing and touch-first interaction.

## Features

- Browse news from the New York Times API
- Enable or disable news categories
- Swipe through articles with touch-friendly interactions
- Save and remove articles from a personal archive
- Persist onboarding state and other preferences in the browser
- Light and dark theme
- Mobile-first responsive interface
- Client-side routing between application views
- Reusable API-fetching logic with loading, error and cache handling

## What this project demonstrates

Newsify separates shared application state from page-level UI concerns. `CategoryContext` and `ArchiveContext` provide state across routes without prop drilling, while the custom `useFetch` hook centralizes API requests, loading states, errors and a time-limited browser cache.

The project also explores mobile interaction patterns through swipe gestures and keeps relevant client-side state in `localStorage` so parts of the experience persist between visits.

## Tech stack

- React
- JavaScript
- Vite
- Sass
- React Router
- React Context
- React Swipeable
- Vitest
- New York Times API
- Netlify

## Architecture highlights

- **Shared state:** `CategoryContext` and `ArchiveContext`
- **Reusable data fetching:** custom `useFetch` hook
- **Persistence:** browser `localStorage`
- **Routing:** React Router
- **Interaction:** swipe gestures with React Swipeable
- **Styling:** component-oriented Sass
- **Testing:** Vitest, with existing component test coverage

## Run locally

### Prerequisites

- Node.js
- A New York Times API key

```bash
git clone https://github.com/ReedorReed/project-newsify.git
cd project-newsify
npm install
```

Create a `.env` file in the project root:

```env
VITE_API_KEY=your_new_york_times_api_key
```

Then start the development server:

```bash
npm run dev
```

## Available commands

```bash
npm run dev      # Start the Vite development server
npm run build    # Create a production build
npm run lint     # Run ESLint
npm run preview  # Preview the production build
```

## Project structure

```text
src/
├── assets/
├── components/
├── context/
├── pages/
├── style/
├── App.jsx
└── main.jsx
```

## Further development

Areas I would improve next include:

- More comprehensive automated testing
- Stronger loading and error states
- Improved accessibility
- Search and additional filtering
- Further refinement of animations and swipe interactions

## Documentation

The repository also contains [technical project documentation](./documentation.md) describing implementation choices made during development.

## Author

**Christian Reed** — Web Developer

- [Portfolio](https://www.reed.dk/)
- [GitHub](https://github.com/ReedorReed)
