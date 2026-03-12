# AI_RULES.md

## Tech Stack Overview

- **Frontend Framework:** React (with TypeScript)
- **Routing:** React Router (routes are defined in `src/App.tsx`)
- **Styling:** Tailwind CSS for all custom styles and layout
- **Component Library:** shadcn/ui (Radix UI-based, pre-installed)
- **Icons:** lucide-react (for all icon needs)
- **Font:** Satoshi via Fontshare (imported in `index.html`)
- **Pages Directory:** All pages go in `src/pages/`
- **Components Directory:** All reusable components go in `src/components/`
- **Main Page:** The default landing page is `src/pages/Index.tsx`
- **Image Assets:** Place images in the project root or a dedicated `public/` folder

## Library Usage Rules

- **UI Components:**  
  - Always use shadcn/ui components for buttons, dialogs, forms, modals, etc.
  - Do NOT modify shadcn/ui source files; create wrappers or new components in `src/components/` if customization is needed.

- **Styling:**  
  - Use Tailwind CSS utility classes for all custom styling and layout.
  - Do not use plain CSS or CSS-in-JS except for global styles in `index.html` or Tailwind config.

- **Icons:**  
  - Use lucide-react for all icons.
  - Do not use SVGs or other icon libraries directly.

- **Routing:**  
  - Use React Router for all navigation.
  - Keep all route definitions in `src/App.tsx`.

- **State Management:**  
  - Use React's built-in state and context APIs.
  - Do not add Redux, Zustand, or other state libraries unless explicitly required.

- **Notifications/Toasts:**  
  - Use shadcn/ui's toast system or `react-hot-toast` if more flexibility is needed.

- **Forms:**  
  - Use shadcn/ui form components.
  - For validation, prefer `react-hook-form` if advanced validation is needed.

- **Responsiveness:**  
  - All components and pages must be responsive using Tailwind's responsive utilities.

- **New Packages:**  
  - Only add new npm packages if absolutely necessary and not already covered by the above stack.