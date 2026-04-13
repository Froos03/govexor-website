# Next Steps – Learning & Building Govexor Website

## 🎯 Goal

Build a **premium, SEO-friendly landing page** using Next.js while learning only what is necessary.

---

## 🧠 What to Focus On (Core Concepts Only)

### 1. App Router (CORE)

Understand how routing works in Next.js.

* `/app/page.tsx` → homepage
* `/app/about/page.tsx` → `/about` route

👉 Keep it simple. This is your foundation.

---

### 2. Layouts (`layout.tsx`)

Controls global structure of your app.

Use it for:

* Navbar
* Footer
* SEO metadata

**Mental model:**

```tsx
<html>
  <body>
    <Navbar />
    {children}
    <Footer />
  </body>
</html>
```

---

### 3. Components

Break your UI into reusable parts.

Examples:

* Hero
* Services
* CTA

```tsx
export default function Hero() {
  return <section>Hero</section>;
}
```

---

### 4. Styling (Tailwind CSS)

Use utility classes instead of writing CSS.

Example:

```tsx
<div className="flex items-center justify-between p-6">
```

Focus on:

* spacing (`p-6`, `m-4`)
* layout (`flex`, `grid`)
* typography (`text-xl`, `font-bold`)

---

### 5. Metadata (SEO 🔥 IMPORTANT)

Add this in `layout.tsx`:

```ts
export const metadata = {
  title: "Govexor - Premium Websites",
  description: "We build SEO-optimized websites for businesses",
};
```

👉 This directly affects Google ranking.

---

### 6. Images (`next/image`)

Use optimized images for performance.

```tsx
import Image from "next/image";

<Image src="/hero.png" width={500} height={500} alt="Hero" />
```

---

### 7. Links (`next/link`)

For navigation between pages.

```tsx
import Link from "next/link";

<Link href="/about">About</Link>
```

---

## ❌ Ignore For Now

Do NOT focus on:

* API routes
* Server Actions
* Middleware
* Authentication
* Databases
* Edge functions
* Advanced caching

👉 These are not needed for a landing page.

---

## 🧭 Learning Strategy (IMPORTANT)

Do NOT read everything.

### Use this method:

1. Read a concept (5–10 minutes)
2. Apply it immediately in code
3. Move to the next concept

---

## 🔥 Practical Plan

### Day 1

* Learn App Router basics
* Understand `layout.tsx` and `page.tsx`
* Run project locally

👉 Goal: Render a basic page

---

### Day 2

* Learn Components
* Learn Tailwind basics

👉 Goal: Build Hero section

---

### Day 3

* Add Metadata (SEO)
* Add Images

👉 Goal: Improve design + SEO

---

## 🧠 Key Mindset

You don’t learn Next.js first.

👉 You learn it WHILE building.

---

## 🚀 Next Action

Start with:

* Create empty homepage
* Add basic layout
* Prepare for Hero section

Then move into building your first real UI section.

---
