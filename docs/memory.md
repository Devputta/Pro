# Project Memory & Decision Log

## Decision 1: CDN-Based Frameworks vs. Heavy Build Tools
- **Context:** Wanted instant preview and zero-friction deployment without complex Webpack/Vite bundlers for this static showcase.
- **Decision:** Utilized Tailwind CSS via CDN script and vanilla JavaScript with Lucide icons.
- **Trade-off:** Faster setup and easier embedding, slightly less tree-shaking control (mitigated by minimal usage).

## Decision 2: Simulated Mobile Frame over External Viewport iframe
- **Context:** Needed a reliable way to show mobile app layouts without CORS restriction issues from external iframe URLs.
- **Decision:** Built a native interactive DOM state switcher inside a CSS-crafted phone frame.
- **Outcome:** Instant layout switching with zero loading lag or external security blockages.
