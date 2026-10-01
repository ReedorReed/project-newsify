# Newsify

Newsify is a mobile-first news application built with React. It uses the New York Times API to let users browse news, choose categories and save articles to a personal archive.

[View the live application](https://reeds-newsify.netlify.app/)

Created during my Web Developer education, this project is included in my portfolio because it demonstrates frontend application design beyond a simple API fetch: shared state, custom hooks, persistence, routing and touch-first interaction.

## Features

- Browse news from the New York Times
- Choose between different news categories
- Swipe to save or remove articles
- View saved articles in an archive
- Customize which news categories are displayed
- Light and dark theme
- Cache API responses and persist saved articles in the browser
- Onboarding flow for first-time users
- Mobile-first responsive design

## Technologies

- React
- JavaScript
- Vite
- Sass with BEM-style component organisation
- New York Times API
- React Router
- React Context and a custom `useFetch` hook
- React Swipeable
- Vitest and Testing Library

## Getting Started

Clone the repository:

```bash
git clone <repository-url>
```

Navigate to the project:

```bash
cd project-newsify
```

Install dependencies:

```bash
npm install
```

Start the development server:

```bash
npm run dev
```

## Environment Variables

The project uses the New York Times API.

Create a `.env` file in the root of the project and add your API key:

```env
VITE_NYT_API_KEY=your_api_key_here
```

You can get an API key from the New York Times Developer Portal.

> Never commit your API key to GitHub.

## Project Structure

```text
src/
├── assets/
├── components/
├── pages/
├── App.jsx
└── main.jsx
```

The application is divided into reusable components and separate pages to keep the project easier to maintain and develop.

## Architecture choices

- `CategoryContext` and `ArchiveContext` hold state that is shared across routes without prop drilling.
- The reusable `useFetch` hook handles loading, errors and a time-limited browser cache for API requests.
- Saved articles and cached responses are stored in `localStorage`, so the experience persists between visits.
- Components own their Sass files, keeping visual concerns close to the interface they support.

## Future Improvements

Possible improvements include:

- Better loading and error states
- Search functionality
- More filtering options
- Improved animations and swipe interactions
- Persisting user preferences and saved articles
- Improved accessibility
- More comprehensive testing

## Author

**Christian Reed** — Web Developer
