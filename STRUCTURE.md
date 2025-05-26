# 📁 Project Structure

> ⚠️ **Note:** This document is a work in progress and may change as the project evolves.

This structure is based on a **ReactJS** project using **TailwindCSS** for styling and **React Router** for routing.

## 📦 Folder Overview

```
/app
├── /assets            → Static files like images, fonts, etc.
├── /components        → Reusable UI components
│   ├── /Component1    → Folder for each individual component
│   │    └── index.tsx → Main component file
│   ├── /Component2
│   └── /Icons         → SVG icons as React components
│        ├── Icon1.tsx
│        ├── Icon2.tsx
│        └── index.ts  → Exports all icons for easy import
├── /data              → Static data and configuration files
│   ├── common.ts      → Reusable data shared across components
│   └── index.ts       → Index file for centralizing exports
├── /routes            → Route-related components and logic
├── app.css            → Global TailwindCSS styles
├── root.tsx           → Main layout/root component
└── routes.ts          → React Router definitions
/public                → Public assets accessible via URL
/references            → Research materials or documentation
```

<br />

## 📁 Detailed Breakdown

### `/app/assets`

Used for static files such as images, fonts, and any raw assets.

### `/app/components`

Contains all reusable components, including general UI components and icons.

- Each component resides in its own folder with its own `index.tsx`.
- The `Icons` folder contains SVG-based React components. The `index.ts` file re-exports them for easier importing.

### `/app/data`

Contains static or shared data such as arrays or objects, centering the exporting on `index.ts`.

### `/app/routes`

Used for storing components or layouts that are directly tied to routing (like pages or views).

### `/app/root.tsx`

Serves as the root layout for the application. Contains the main structure of the app and wraps routing.

### `/app/routes.ts`

Routes definitions using React Router. Helps organize navigation logic.

### `/app.css`

Main global stylesheet, typically where Tailwind is declared.

### `/public`

Contains files that should be publicly accessible, such as favicon or preview images.

### `/references`

Optional folder used for storing helpful links, inspiration, or project-related documentation.

<br />

## ✅ Best Practices

- Use PascalCase for component folders and files (e.g., `ComponentName/index.tsx`).
- Use camelCase or snake_case for files that are not components (e.g., `common.ts`, `routes.ts`).
- Keep shared data and utilities centralized (e.g., via `/data/index.ts`).
- Export from `index.ts` files when possible for cleaner imports.
- Separate route logic (`routes.ts`) from the root layout (`root.tsx`).

<br />

Go back to the project documentation on [`README.md`](README.md).
