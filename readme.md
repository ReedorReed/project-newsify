# Newsify

Newsify is a mobile-first news application built with React. The app fetches news articles from the New York Times API and allows users to browse different news categories, save interesting articles, and manage their own archive.

The project was created as part of my Web Developer education and focuses on working with APIs, React components, state management, routing, and responsive UI development.

## Features

- Browse news from the New York Times
- Choose between different news categories
- Swipe to save or remove articles
- View saved articles in an archive
- Customize which news categories are displayed
- Light and dark theme
- Mobile-first responsive design

## Technologies

- React
- JavaScript
- Vite
- CSS / SCSS
- New York Times API
- React Router
- Git & GitHub

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

## What I Learned

During this project I worked with:

- Fetching and displaying data from an external API
- Managing state in React
- Passing data between components
- Creating reusable React components
- Working with React Router
- Implementing user interactions such as saving and removing articles
- Building a responsive mobile-first interface
- Implementing light and dark themes
- Structuring a larger React application

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

**Christian Reed**

Web Developer student at Roskilde Tekniske Skole.
