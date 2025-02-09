# Blank Screen on Initial Load with Client-Side Routing in Next.js 15

This repository demonstrates a bug in Next.js 15 where a client-side-routed application shows a blank screen on the initial load.  The issue is resolved by ensuring the `pages/index.js` file is properly configured to render content on the initial load.

## Bug Description

A Next.js 15 application using client-side routing displays a blank screen initially.  The About page renders correctly after navigating from the Home page. This indicates a problem with initial rendering of the Home page.

## How to Reproduce

1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npm run dev` to start the development server.
4. Observe that the initial page is blank.  Navigate to the '/about' page and observe that the page renders without issues.  

## Solution

The problem stems from a missing or improperly formatted initial route.  The solution involves ensuring the main `pages/index.js` component has content to render initially.  No additional configuration is required beyond proper component creation.