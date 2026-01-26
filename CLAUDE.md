# Next.js Project

This is a Next.js 15 application with the App Router and TypeScript.

## Commands

- `npm run dev` - Start dev server on port 3000
- `npm test` - Run tests
- `npm run lint` - Run ESLint
- `npm run build` - Build for production

## Architecture

- **App Router** in `app/` - File-based routing with layouts
- **Server Components** are the default - use `'use client'` only when needed
- **API Routes** in `app/api/` for backend endpoints
- **Components** in `components/` are reusable UI components

## Conventions

- Prefer Server Components for data fetching
- Use Server Actions for mutations when possible
- Keep client components small and focused on interactivity
- Use `loading.tsx` and `error.tsx` for loading/error states
- Colocate component files with their page when page-specific

## Data Fetching

- Fetch data in Server Components directly with `async/await`
- Use `fetch()` with Next.js caching options
- For client-side data, use React Query or SWR
