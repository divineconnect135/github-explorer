# GitHub Explorer

A responsive GitHub user search application built with React, TypeScript, Vite, and TanStack Query.

GitHub Explorer allows users to search for GitHub accounts, view profile information, get live search suggestions, and access recent searches.

## Live Demo

[View Live Demo](https://github-explorer-seven-bice.vercel.app/)

## Features

- Search GitHub users by username
- Live search suggestions
- Debounced search input
- View GitHub profile information
- Recent search history
- Persistent recent searches using localStorage
- Loading states
- Error handling
- API response caching
- Query prefetching
- Automatic refetching
- Type-safe API handling with TypeScript
- Responsive design

## Tech Stack

- React
- TypeScript
- Vite
- TanStack Query
- TanStack Query Devtools
- GitHub REST API
- use-debounce
- localStorage
- CSS

## Technical Implementation

### GitHub REST API

The application uses the GitHub REST API to search for users and retrieve GitHub profile information.

### Server State Management

TanStack Query is used to manage API-related server state, including:

- Data fetching
- Response caching
- Loading states
- Error states
- Refetching
- Prefetching
- Query lifecycle management

Each GitHub user is cached using a unique query key.

```ts
queryKey: ["users", username]
