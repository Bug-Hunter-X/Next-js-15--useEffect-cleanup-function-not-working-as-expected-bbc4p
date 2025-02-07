# Next.js 15 useEffect Cleanup Issue

This repository demonstrates a problem with the `useEffect` hook's cleanup function in a Next.js 15 application.  A counter on the About page continues to increment even after leaving the page, indicating that the cleanup function isn't properly clearing the interval.

## Bug Report

The `about.js` file contains a counter that increments every second.  A `useEffect` hook is used to set up and clear the interval.  However, the counter keeps incrementing when navigating away from the About page.

## Solution

The `aboutSolution.js` file provides a corrected implementation.  The issue was resolved by ensuring the cleanup function was properly called and the interval was cleared.