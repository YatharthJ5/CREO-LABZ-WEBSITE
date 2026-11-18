# CREO LABZ — premium animation upgrade
Single-page static site (index.html). Logo embedded and also in assets/.
Run: open index.html, or `npm start` (needs network for npx serve).
Deploy: upload index.html to any static host (Netlify, Vercel static, S3, cPanel).
Needs internet for three.js (cdnjs) and Manrope (Google Fonts).
Enquiry backend: see .env.example.

## Engineering improvements
- Responsive navigation, project overlays, and enquiry dialog include keyboard focus and reduced-motion support.
- The Three.js construction scene pauses outside the build section, adapts pixel density for mobile, and handles WebGL context loss/restoration.
- Scroll and reveal effects avoid continuous work outside the active 3D scene.
- Local assets and static hosting remain unchanged; no build step or extra runtime dependency is required.
