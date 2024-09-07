
![Screenshot 2024-09-06 at 16 57 25](https://github.com/user-attachments/assets/d6d0c53e-5b3e-4d49-b6e8-1dfbc6808a0f) ![Screenshot 2024-09-06 at 16 57 51](https://github.com/user-attachments/assets/ce94c628-8103-44d0-ae0e-4f7dc184f404) ![Screenshot 2024-09-06 at 16 58 10](https://github.com/user-attachments/assets/794bde3c-d08d-43cc-9e49-eb44033fe4a6) ![Screenshot 2024-09-06 at 16 58 17](https://github.com/user-attachments/assets/3ae53a9c-7908-4e09-bdbf-0e922a436789) ![Screenshot 2024-09-06 at 16 58 30](https://github.com/user-attachments/assets/77398251-b28d-4194-a27c-52690589d3bf) ![Screenshot 2024-09-06 at 16 58 48](https://github.com/user-attachments/assets/cf804485-b6ad-4fa3-8040-9a26fe7845b9) ![Screenshot 2024-09-06 at 16 59 46](https://github.com/user-attachments/assets/98b2b40f-d2fc-4c03-bead-d80b91fc1ed9)


## FreeScribe-ML-React-WebApp

FreeScribe is a Machine Learning (ML) React Vite TailwindCSS Web Based Transcription and Translation App that uses Web Workers to run ML models in the browser. This app allows you to record your voice or upload an audio file (mp3/wav), transcribe it to text, translate it into any language, and download or copy the freshly converted text that has been transcribed and deployed on Vercel. This kind of app is essential and expensive in the IT manufacturing field, but it's integrated here smoothly, shared, and at no cost.

**Note: To check this web app live, click here:** https://free-scribe-arnob.vercel.app/

## To Install Dependences

Before launching this web application, be sure to install all required dependencies, which are listed in the package.json file.

To install all dependences, run this command from your project folder: `npm install`

## To Install NodeJS

Make sure you have NodeJS installed in your machine first, The installation instructions are here: https://nodejs.org/en/

## To Create TailwindCSS React Vite Project

Open up your terminal and bootstrap a new React Vite App by: `npm create vite@latest my-project -- --template react`

Then go to that project folder, and write this command via terminal from your project folder: `npm install -D tailwindcss postcss autoprefixer`

Then install tailwindcss and its peer dependencies, then generate your `tailwind.config.js` and `postcss.config.js` files: `npx tailwindcss init -p`

Then add the paths to all of your template files in your tailwind.config.js file.

```
/** @type {import('tailwindcss').Config} */
export default {
  content: [
    "./index.html",
    "./src/**/*.{js,ts,jsx,tsx}",
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

Then add the @tailwind directives for each of Tailwind’s layers to your ./src/index.css file.

```
@tailwind base;
@tailwind components;
@tailwind utilities;
```

Run your project: `npm run dev`

Run on your browser Local: `http://localhost:5173/`

(For more details, visit: https://tailwindcss.com/docs/guides/vite )

## To Install `@xenova/transformers`

Run this command via terminal from your project folder: `npm i @xenova/transformers`

(For more details, visit: https://github.com/xenova/transformers.js )

## About presets.js File

I copied that presets.js file from GitHub. Its pretty same to use for transcription and translation overall. Here I used web worker as well.

