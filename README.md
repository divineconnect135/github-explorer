# GitHub Explorer

A GitHub user search application built with **React, TypeScript, Vite, and TanStack Query**. Search GitHub users, view profile information, get live suggestions, and access recent searches.

## Features

* Search GitHub users by username
* Live user suggestions
* Debounced search requests
* GitHub profile details
* Recent search history with `localStorage`
* Loading and error handling
* TanStack Query caching
* Query prefetching and refetching
* TanStack Query Devtools
* TypeScript type safety

## Tech Stack

* React
* TypeScript
* Vite
* TanStack Query
* TanStack Query Devtools
* GitHub REST API
* use-debounce
* CSS

## Project Structure

```text
src/
├── api/
│   └── github.ts
├── components/
│   ├── RecentSearches.tsx
│   ├── SuggestionDropdown.tsx
│   ├── UserCard.tsx
│   └── UserSearch.tsx
├── App.tsx
├── index.css
├── main.tsx
└── types.ts
```

## TanStack Query

TanStack Query handles server-state management, including:

* Fetching GitHub data
* Caching responses
* Loading and error states
* Refetching
* Prefetching
* Query invalidation and lifecycle management

Queries are identified using query keys such as:

```tsx
queryKey: ["users", username]
```

This allows GitHub users to be cached independently.

## Run Locally

Install dependencies:

```bash
npm install
```

Start the development server:

```bash
npm run dev
```

## Environment Variables

Create a `.env` file if required:

```env
VITE_GITHUB_TOKEN=your_github_token
```

Do not commit your `.env` file or expose sensitive credentials in a public repository.

## GitHub API

This project uses the GitHub REST API for user profiles and user search.

## Purpose

This project demonstrates practical usage of **React + TypeScript** with **TanStack Query** for efficient server-state management, caching, debouncing, prefetching, and refetching.
