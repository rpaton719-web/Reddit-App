# vite-template-redux

The official Redux + TypeScript template for [Vite](https://vite.dev/). Uses [Redux Toolkit](https://redux-toolkit.js.org/), [React Redux](https://react-redux.js.org/), [Vitest](https://vitest.dev/), and [React Testing Library](https://testing-library.com/docs/react-testing-library/intro/).

```sh
npx tiged reduxjs/redux-templates/packages/vite-template-redux my-app
cd my-app
npm install
```

Or try it in the browser: [Open in StackBlitz](https://stackblitz.com/github/reduxjs/redux-templates/tree/master/packages/vite-template-redux)

The `overrides` field in `package.json` pins `rolldown` to 1.2.8 because 1.2.9 crashes on startup inside StackBlitz's WebContainer ([stackblitz/webcontainer-core#2167](https://github.com/stackblitz/webcontainer-core/issues/2167)). It has no effect in the pnpm workspace; npm applies it when the folder is installed on its own. Remove it once rolldown ships a fix.

## What's inside

- `src/app/store.ts` - the Redux store, set up with `combineSlices` and `configureStore`, plus a `makeStore` factory and the `RootState` / `AppDispatch` types
- `src/app/hooks.ts` - pre-typed `useAppSelector` and `useAppDispatch`
- `src/features/counter` - a `createSlice` example with a thunk, plus tests
- `src/features/quotes` - an RTK Query API slice fetching from a public API
- `src/utils/test-utils.tsx` - a `renderWithProviders` helper for testing components that use the store

Linting and formatting use [oxlint](https://oxc.rs/docs/guide/usage/linter) and [oxfmt](https://oxc.rs/docs/guide/usage/formatter).

## Scripts

- `dev` / `start` - start the dev server
- `build` - build for production
- `preview` - preview the production build locally
- `test` - run the tests once
- `lint` / `lint:fix` - lint with oxlint
- `format` / `format:check` - format with oxfmt
- `type-check` - run the TypeScript compiler without emitting

# Intro

## Build Your Own Reddit App

For this project, you will build an application for Reddit using everything you’ve learned, including React and Redux. Reddit is a website where people share links to articles, media and other things on the web. The Reddit API provides data which you will integrate into your application. The application will allow users to view and search posts and comments provided by the API.

### Example Project

See Reddit App Soln (local file) for a completed example.

### Project Requirements

- [ ] Build the application using React and Redux

- [ ] Version control your application with Git and host the repository on GitHub

- [ ] Use a project management tool (GitHub Projects, Trello, etc.) to plan your work

- [ ] Write a README (using Markdown) that documents your project including:
  - [ ] Wireframes
  - [ ] Technologies used
  - [ ] Features
  - [ ] Future work
  - [ ] Write unit tests for your components using Jest and Enzyme

- [ ] Write end-to-end tests for your application

- [ ] Users can use the application on any device (desktop to mobile)

- [ ] Users can use the application on any modern browser

- [ ] Users can access your application at a URL

- [ ] Users see an initial view of the data when first visiting the app

- [ ] Users can search the data using terms

- [ ] Users can filter the data based on categories that are predefined

- [ ] Users are shown a detailed view (modal or new page/route) when they select an item

- [ ] Users are delighted with a cohesive design system

- [ ] Users are delighted with animations and transitions

- [ ] Users are able to leave an error state

- [ ] Get 90+ scores on Lighthouse

  We understand you cannot control how media assets like videos and images are sent to the client. It is okay to have a score below 90 for Performance if they are related to the media from Reddit.

- [ ] OPTIONAL: Get a custom domain name and use it for your application

- [ ] OPTIONAL: Set up a CI/CD workflow to automatically deploy your application when the master branch in the repository changes

- [ ] OPTIONAL: Make your application a progressive web app

### Prerequisites

- HTML
- CSS
- JavaScript
- React
- Redux
- Jest and Selenium
- Git and GitHub
- Command line and file navigation
- Wireframing

# Project Plan

## End Result

Lite Reddit client. A reader that displays subreddit posts on individual cards. Can scroll page to see other cards.

Consider adding up/down vote buttons?

## What is it built with?

- React
- Redux
- CSS

## What can it do?

Display subreddit posts on cards.

## Wireframes

- Black/white colors
- Cards center of page, arranged vertically

## Features

## Timeline

- [ ] Wireframe project (15m)
- [ ] Set up version control (5m)
- [ ] Bootstrap with `Vite` (10m)
- [ ] Build components ()
- [ ] Write tests
- [ ] Add Reddit data / implement Reddit API ()
- [ ] Publish to the web ()
- [ ] Next steps (see README)

# Future Work

- [ ] Finish the project
- [ ] Implement optional features
  - [ ] OPTIONAL: Get a custom domain name and use it for your application

  - [ ] OPTIONAL: Set up a CI/CD workflow to automatically deploy your application when the master branch in the repository changes

  - [ ] OPTIONAL: Make your application a progressive web app
