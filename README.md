<h3 align="center">Real Time Figma Clone MERN Stack Project</h3>

## 📋 <a name="table">Table of Contents</a>

1. 🗽 [Authors](#authors)
2. 🤖 [Introduction](#introduction)
3. ⚙️ [Tech Stack](#tech-stack)
4. 🔋 [Features](#features)
5. 🤸 [Quick Start](#quick-start)
6. 🕸️ [Snippets](#snippets)
7. 🖼️ [Screenshots](#screenshots)
8. 🎥 [Video](#video)

## <a name="authors"> 🗽 Authors:</a>

*1. Chanchal Rajput*
- Roll no.-22015002561
- Sec: C
- Batch: 2 (Second)

*1. Shlok Agarwal*
- Roll no.-22015002871
- Sec: G
- Batch: 2 (Second)


## <a name="introduction">🤖 Introduction</a>

A minimalistic Figma clone to show how to add real-world features like live collaboration with cursor chat, comments, reactions, and drawing designs (shapes, image upload) on the canvas using fabric.js.

## <a name="tech-stack">⚙️ Tech Stack</a>

- Next.js
- TypeScript
- Liveblocks
- Fabric.js
- Shadcn
- Tailwind CSS

## <a name="features">🔋 Features</a>

👉 *Multi Cursors, Cursor Chat, and Reactions*: Allows multiple users to collaborate simultaneously by showing individual cursors, enabling real-time chat, and reactions for interactive communication.

👉 *Active Users*: Displays a list of currently active users in the collaborative environment, providing visibility into who is currently engaged.

👉 *Comment Bubbles*: Enables users to attach comments to specific elements on the canvas, fostering communication and feedback on design components.

👉 *Creating Different Shapes*: Provides tools for users to generate a variety of shapes on the canvas, allowing for diverse design elements

👉 *Uploading Images*: Import images onto the canvas, expanding the range of visual content in the design

👉 *Customization*: Allows users to adjust the properties of design elements, offering flexibility in customizing and fine-tuning visual components

👉 *Freeform Drawing*: Enables users to draw freely on the canvas, promoting artistic expression and creative design.

👉 *Undo/Redo*: Provides the ability to reverse (undo) or restore (redo) previous actions, offering flexibility in design decision-making

👉 *Keyboard Actions*: Allows users to utilize keyboard shortcuts for various actions, including copying, pasting, deleting, and triggering shortcuts for features like opening cursor chat, reactions, and more, enhancing efficiency and accessibility.

👉 *History*: Review the chronological history of actions and changes made on the canvas, aiding in project management and version control.

👉 *Deleting, Scaling, Moving, Clearing, Exporting Canvas*: Offers a range of functions for managing design elements, including deletion, scaling, moving, clearing the canvas, and exporting the final design for external use.

and many more, including code architecture, advanced react hooks, and reusability 

## <a name="quick-start">🤸 Quick Start</a>

Follow these steps to set up the project locally on your machine.

*Prerequisites*

Make sure you have the following installed on your machine:

- [Node.js](https://nodejs.org/en)
- [npm](https://www.npmjs.com/) (Node Package Manager)


*Installation*

Install the project dependencies using npm:

bash
npm install


*Set Up Environment Variables*
-
Create a new file named .env.local in the root of your project and add the following content:

```bash
env
NEXT_PUBLIC_LIVEBLOCKS_PUBLIC_KEY = 
```

Replace the placeholder values with your actual Liveblocks credentials. You can obtain these credentials by signing up on the [Liveblocks website](https://liveblocks.io).

*Running the Project*

bash
npm run dev

![Run_in_Terminal](https://github.com/Shri-Shlok-Agarwal/Project_MERN_Stack/assets/139161753/d552159d-64b3-4ad3-97ff-1f3c2ef3d84f)

Open [http://localhost:3000](http://localhost:3000) in your browser to view the project.

## <a name="snippets">🕸️ Snippets</a>

### Styles

<details>
<summary><code>tailwind.config.ts</code></summary>

typescript
import type { Config } from "tailwindcss";

const config = {
  darkMode: ["class"],
  content: [
    "./pages/**/*.{ts,tsx}",
    "./components/**/*.{ts,tsx}",
    "./app/**/*.{ts,tsx}",
    "./src/**/*.{ts,tsx}",
  ],
  prefix: "",
  theme: {
    container: {
      center: true,
      padding: "2rem",
      screens: {
        "2xl": "1400px",
      },
    },
    extend: {
      colors: {
        primary: {
          black: "#14181F",
          green: "#56FFA6",
          grey: {
            100: "#2B303B",
            200: "#202731",
            300: "#C4D3ED",
          },
        },
      },
      keyframes: {
        "accordion-down": {
          from: { height: "0" },
          to: { height: "var(--radix-accordion-content-height)" },
        },
        "accordion-up": {
          from: { height: "var(--radix-accordion-content-height)" },
          to: { height: "0" },
        },
      },
      animation: {
        "accordion-down": "accordion-down 0.2s ease-out",
        "accordion-up": "accordion-up 0.2s ease-out",
      },
    },
  },
  plugins: [require("tailwindcss-animate")],
} satisfies Config;

export default config;


</details>

<details>
<summary><code>app/globals.css</code></summary>

css
@tailwind base;
@tailwind components;
@tailwind utilities;

@import "@liveblocks/react-comments/styles.css";

* {
  font-family:
    work sans,
    sans-serif;
}

@layer utilities {
  .no-ring {
    @apply outline-none ring-0 ring-offset-0 focus:ring-0 focus:ring-offset-0 focus-visible:ring-offset-0 !important;
  }

  .input-ring {
    @apply h-8 rounded-none border-none  bg-transparent outline-none ring-offset-0 focus:ring-1  focus:ring-primary-green focus:ring-offset-0 focus-visible:ring-offset-0 !important;
  }

  .right-menu-content {
    @apply flex w-80 flex-col gap-y-1 border-none bg-primary-black py-4 text-white !important;
  }

  .right-menu-item {
    @apply flex justify-between px-3 py-2 hover:bg-primary-grey-200 !important;
  }
}


</details>

## <a name="screenshots"> 🖼️ Screenshots:</a>

*Loading Page*
-
![Screenshot_1](https://github.com/Shri-Shlok-Agarwal/Project_MERN_Stack/assets/139161753/deb3fbb2-933d-4236-b71f-91f3c0040f52)

*Home Page*
-
![Screenshot_2](https://github.com/Shri-Shlok-Agarwal/Project_MERN_Stack/assets/139161753/4a4bd478-6f68-407a-a0c0-d95141ea5245)


## <a name="video"> 🎥 Video:</a>

*Our Project Tour*
-
https://github.com/Shri-Shlok-Agarwal/MernStack_Project/assets/139161753/9e124790-6bd1-4e4f-859c-00f9838a0559
