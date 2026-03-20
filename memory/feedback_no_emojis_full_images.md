---
name: design feedback — no emojis, full images, logo
description: User preferences for visual design on Prep LoCal website and future projects
type: feedback
---

Never use emojis in code or UI. Replace all emoji icons with proper SVG icons or styled HTML elements.

**Why:** User explicitly corrected this twice. Emojis look unprofessional and inconsistent across platforms.

**How to apply:** Any time an icon is needed (calendar, check, truck, etc.), use an inline SVG or a Unicode symbol like ✓ only if it's a legitimate typographic character — never use emoji like 📅 🚗 🍗.

---

Always show food/product images at full size with no cropping. Use `width: 100%; height: auto;` so the full image is visible.

**Why:** User explicitly asked for "bigger pictures so you can see everything in the picture no cutoffs."

**How to apply:** Do not use `object-fit: cover` with a fixed height on food images. Let them render at their natural aspect ratio. Use `object-fit: contain` only if a fixed container is necessary.

---

Always verify image-to-label mapping before assigning photos to named items. Read the images to confirm what food is actually shown before labeling.

**Why:** Wrong image was showing under a food name (salmon showing next to chicken label due to hero card layout).

**How to apply:** Before building a menu/product section, read every image file and note what it shows. Never guess based on filename order.
