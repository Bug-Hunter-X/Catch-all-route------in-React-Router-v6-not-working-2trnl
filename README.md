# React Router v6 Catch-all Route Issue

This repository demonstrates a problem with the catch-all route (`/*`) in React Router v6.  Other routes are working correctly, but the catch-all route fails to render when a path doesn't match any other defined routes.

## Problem

The `/*` route, intended to act as a 404 Not Found page, is not rendering.  This issue prevents the application from gracefully handling undefined routes.

## Solution

The solution involves modifying the order of routes. By placing the catch-all route last, React Router can correctly match it when no other route is found.