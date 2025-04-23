# Inspirational Quotes

A React & TypeScript example app that displays random and paginated inspirational quotes. It uses MirageJS to mock a RESTful API with endpoints for fetching all quotes.

## Features
- **Mock API** powered by MirageJS
  - GET /api/quotes?limit=<n>&offset=<m> – fetch a slice of quotes
  - GET /api/quotes/random – fetch one random quote, shuffled via Lodash 
  - Full CRUD routes (POST, PATCH, DELETE) stubbed out for further extension 

- **Quote Components**
  - InspirationalQuote – displays a single quote with optional source 
  - Quotes – form to load a user-specified number of quotes and grid layout for display 
  - Loading – full-screen loader with Tailwind CSS animation 

- **Filtering** (in src/lib/filter-quotes.ts) to narrow quotes by content or source using simple client-side logic 
- **TypeScript** typings for strong type safety (e.g. Quote type in application.tsx) 
- **Styling with Tailwind CSS** for utility-first responsive design

## Tech Stack
- **React** (v18.2.0) & **React DOM**
- **TypeScript** for type-safe components 
- **MirageJS** (v0.1.46) for in-browser API mocking 
- **Lodash.shuffle** for randomization 
- **Tailwind CSS** for styling and layout 
- **React Scripts** for build tooling 
- **UUID, clsx, prop-types** (optional utilities)

## Installation
1. Clone the repo
   ```bash
    git clone https://github.com/abrun-s/inspirational-quotes.git
    cd inspirational-quotes
2. Install dependencies
   ```bash
    npm install
3. Run the development server
   ```bash
    npm start
