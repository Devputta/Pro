# Architecture Document

## 1. System Overview
The application follows a client-side rendered (CSR) single-page architecture built for maximum portability and instant deployment on static hosting platforms (Vercel / GitHub Pages).

## 2. Component Topology
```
[ Client Browser ] 
       │
       ├──> index.html (Tailwind CSS CDN + Lucide Icons)
       │         │
       │         ├──> Navbar & Hero Header
       │         ├──> Featured Repositories Grid
       │         └──> Interactive Mobile Viewer (DOM State Switcher)
       │
       └──> External Assets & GitHub API Links
```

## 3. Data Flow
1. User loads the web application.
2. Tailwind CSS parses styling rules locally.
3. Lucide icons initialize on DOMContentLoaded.
4. User interacts with the mobile simulator buttons, triggering JavaScript event handlers (`switchScreen()`) to update the container DOM state dynamically.
