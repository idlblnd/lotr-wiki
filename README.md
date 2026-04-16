# LOTR Wiki

A Lord of the Rings themed wiki experience built with React, Vite, React Router, and Tailwind CSS. The project uses the public [The One API](https://the-one-api.dev/) to present movies, books, chapters, characters, and quotes in a more atmospheric archive-style interface.

## Overview

This project was designed to feel less like a plain data table and more like a curated Middle-earth archive. Alongside API-driven pages, it also includes a few extra interactive experiences to make the app feel more complete and polished.

## Highlights

- Public API integration with meaningful UI rendering for:
  - movies
  - movie details
  - books
  - book chapters
  - characters
  - quotes
- Shared loading, error, and empty states for a more consistent user experience
- Cached API responses inside a custom `useFetch` hook to reduce repeated loading delays
- Search, filtering, and sorting features across multiple pages
- Route-based navigation with active states and a mobile navigation menu
- Additional creative features including:
  - memory game
  - journey builder
  - lore quiz

## Tech Stack

- React 19
- Vite
- React Router
- Tailwind CSS


## Folder Structure

```text
src/
  assets/       static images and media
  components/   reusable UI pieces
  hooks/        shared custom hooks
  pages/        route-level views
  services/     API request helpers
```

## Features in Practice

### API Integration and Data Handling

- Data is fetched from The One API through centralized helpers in `src/services/api.js`
- The custom `useFetch` hook manages:
  - loading state
  - error state
  - normalized response data
  - cached repeat requests
- API responses are used directly in lists, detail pages, counters, and filtered views

### React Architecture

- Route pages are kept inside `src/pages`
- Shared UI is separated into `src/components`
- Reusable data logic is moved into `src/hooks`
- Props and local state are used to keep page behavior modular and readable

## Quality Notes

- Tailwind CSS is used throughout the project for styling
- Repeated feedback states were refactored into shared components
- Comments are kept light and intentional so the code still feels clean

## Author

Designed and developed by İdil Balandı.
