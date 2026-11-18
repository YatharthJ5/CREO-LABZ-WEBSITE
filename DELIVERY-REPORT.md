# Delivery report
Added: word-by-word heading reveals, scroll-aware header, animated mobile menu, six concept projects (clip-mask reveals, parallax, hover, cursor label, detail overlay with 3-image gallery), 5-step enquiry (state kept, validation, review/edit, honest WhatsApp fallback), floating WhatsApp button, rebuilt footer, focus states, reduced-motion support.
Tested (headless Chromium, 1440x900): enquiry flow end-to-end, validation, project overlay + gallery arrows, no script errors. Not tested: 3D scene in this run (CDN blocked in sandbox), mobile devices, phone/email links, real backend.
Not done: Next.js/React project, lockfile, separate project/service pages, photography.

## Upgrade QA pass
- Added a main landmark and skip link.
- Replaced invalid project-card button markup with keyboard-operable article cards.
- Added mobile menu aria state, focus movement, and Escape cleanup.
- Reduced 3D rendering outside the build section and added mobile pixel-ratio/camera adjustments.
- Added WebGL context-loss and context-restored handling.
- Added compact mobile spacing, typography, and 320 px safeguards.
- Preserved all existing visual sections, assets, colours, 3D sequence, project overlays, and enquiry fallback.

## Live viewport verification
Passed at 2560x1440, 1920x1080, 1440x900, 834x1194, 768x1024, 430x932, 390x844, 375x812, and 320x720 with no horizontal overflow.

Verified the mobile menu, project overlay, enquiry flow, 5-step review, 3D canvas presence, and reverse-scroll stage logic in headless Chromium. No console or page errors were observed. External Three.js delivery and the real enquiry endpoint remain deployment considerations described in README.md and .env.example.
