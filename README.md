## Features

- ✨ Modern UI with smooth animations and transitions
- 🎯 Responsive and mobile-friendly design
- 🚀 Fast static site powered by Next.js 14
- 🎥 Scroll-based and motion animations using Framer Motion, Locomotive Scroll, and GSAP
- 🧩 Modular component-based architecture
- 📱 Mobile navigation bar and touch-friendly sliders (Swiper)
- 🖼️ SVG icons with React Icons
- 💡 Code splitting and font optimization with next/font
- 🔥 Custom Google Fonts integration
- 🌗 Easy to deploy on Vercel or Netlify

---

## Tech Stack

- **Frameworks**: [Next.js 14](https://nextjs.org/), [React.js](https://react.dev/)
- **Styling**: [TailwindCSS](https://tailwindcss.com/)
- **Animations**: [Framer Motion](https://www.framer.com/motion/), [GSAP](https://greensock.com/gsap/), [Locomotive Scroll](https://github.com/locomotivemtl/locomotive-scroll/)
- **Icons**: [React-Icons](https://react-icons.github.io/react-icons/)
- **Slider**: [Swiper](https://swiperjs.com/)
- **Typography**: [Split-Type](https://github.com/lukePeavey/SplitType), [next/font](https://nextjs.org/docs/basic-features/font-optimization)
- **Type Checking**: TypeScript
- **Other**: ESLint, PostCSS

---

## Project Structure

```
.
├── app/                # Next.js app directory (routes, pages)
├── components/         # Reusable React components
│   ├── About.tsx
│   ├── Badge.tsx
│   ├── Footer.tsx
│   ├── Header.tsx
│   ├── Hero.tsx
│   ├── OpeningHours.tsx
│   ├── Separator.tsx
│   ├── Testimonials.tsx
│   ├── Explore/        # Subcomponents
│   ├── Menu/
│   └── Nav/
├── public/             # Static assets (images, icons)
├── styles/             # Tailwind and global styles
├── .eslintrc.json      # Linting configuration
├── netlify.toml        # Netlify deployment config
├── next.config.mjs     # Next.js configuration
├── package.json        # Project dependencies
├── postcss.config.mjs  # PostCSS config
├── tailwind.config.ts  # TailwindCSS config
├── tsconfig.json       # TypeScript config
└── type.d.ts           # TypeScript type definitions
```

## Key Components

- **Header.tsx**: Top navigation bar, branding, and links.
- **Hero.tsx**: Hero section with eye-catching imagery and main call-to-action.
- **About.tsx**: Info about the coffee shop, mission, and values.
- **Menu/**: Menu component(s) showing products or offerings.
- **Explore/**: Call-to-action and exploration features.
- **Testimonials.tsx**: Customer testimonials with Swiper slider.
- **Footer.tsx**: Closing section with contact info and links.
- **Nav/**: Handles the mobile and desktop navigation.

Each component is written in TypeScript for safety and clarity, and is styled with TailwindCSS utility classes.

---

## How to Run the Project

### 1. Prerequisites

- **Node.js**: Install from [nodejs.org](https://nodejs.org/en/)
- **npm** (comes with Node.js), **yarn**, **pnpm**, or **bun**

### 2. Install Dependencies

```bash
npm install
# or
yarn install
# or
pnpm install
```

You may need to install additional packages:

```bash
npm i gsap react-icons split-type swiper
npm install locomotive-scroll@beta
npm i framer-motion
```

### 3. Start the Development Server

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

---

## API, Routes & Functionality

This project is a **static frontend**—it does not connect to a backend API. All content and interactivity are handled on the client-side using React components and Next.js routing.

- **Routing**: Uses Next.js App Router (`app/` directory). Page editing starts in `app/page.js` or `app/page.tsx`.
- **Fonts**: Uses Next.js `next/font` for Google font optimization.
- **Scroll Animation**: Locomotive Scroll and GSAP provide advanced scroll effects (parallax, smooth scrolling).
- **Sliders**: Swiper.js implements interactive testimonial and product sliders.
- **Responsiveness**: TailwindCSS ensures the site looks great on all devices.
- **Motion/Transitions**: Framer Motion animates elements for engaging UI/UX.

---

## Learning & Examples

### Example: Adding a New Component

Here’s how you might add a new section to the homepage:

```tsx
// components/NewSection.tsx
import React from "react";

export default function NewSection() {
  return (
    <section className="py-12 bg-gray-100">
      <div className="container mx-auto">
        <h2 className="text-3xl font-bold mb-4">Our Special Roasts</h2>
        <p className="text-lg">
          Explore our exclusive coffee blends handpicked by our experts.
        </p>
      </div>
    </section>
  );
}
```

Import and use it in your main page:

```tsx
import NewSection from "@/components/NewSection";

export default function HomePage() {
  return (
    <main>
      {/* ...other sections... */}
      <NewSection />
      {/* ...other sections... */}
    </main>
  );
}
```

### Example: Using Tailwind with Framer Motion

```tsx
import { motion } from "framer-motion";

<motion.div
  className="p-6 bg-white rounded shadow"
  initial={{ opacity: 0, y: 50 }}
  animate={{ opacity: 1, y: 0 }}
  transition={{ duration: 0.5 }}
>
  Animated Section!
</motion.div>;
```

---

## Useful Links & Tutorials

- [Live Demo](https://coffeeshop-arnob.vercel.app/)
- [Next.js Documentation](https://nextjs.org/docs)
- [Learn Next.js](https://nextjs.org/learn)
- [Framer Motion Docs](https://www.framer.com/motion/)
- [Locomotive Scroll Docs](https://scroll.locomotive.ca/docs#/)
- [GSAP Docs](https://greensock.com/gsap/)
- [Swiper Docs](https://swiperjs.com/)
- [TailwindCSS Docs](https://tailwindcss.com/)
- [React Icons](https://react-icons.github.io/react-icons/)
- [Project Tutorial Video](https://www.youtube.com/watch?v=TIbyO-bwdUs)
- [Flex Property Explanation](https://miyattiblog.com/explanation-of-flex-property/)

---

## Deployment

- **Vercel**: Click [here](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app) to deploy on Vercel in seconds.
- **Netlify**: Use `netlify.toml` for Netlify configuration.
- See the [Next.js deployment docs](https://nextjs.org/docs/deployment) for more options.

---

## Keywords

Next.js, React, TailwindCSS, Coffee Shop Website, Framer Motion, Locomotive Scroll, GSAP, Swiper, TypeScript, Static Site, Modern UI, Responsive Design, Web Animations, Component Architecture, Frontend, Web Development, Teaching Project, Learning Resource

---

## Conclusion

This project is a robust example of modern frontend engineering using the React and Next.js ecosystem, packed with animations and best practices in component design, styling, and deployment.  
It is a perfect resource for both learning and teaching advanced frontend concepts, as well as a solid template for real-world coffee shop/business websites.

---

## Happy Coding! 🚀
