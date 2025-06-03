🐾 Animal Explorer
A simple and beautiful web application built with React and Tailwind CSS to explore information about various animals, including their biological names, characteristics, and conservation status.

✨ Features
Animal Search: Easily search for animals by their common name.
Detailed Information: View scientific name, key characteristics (diet, habitat, lifespan, etc.).
Conservation Status: Get the IUCN Red List conservation status for the searched animal.
Responsive Design: A clean and modern interface that looks great on all devices.
API Integration: Fetches data from external APIs for comprehensive information.
🚀 Technologies Used
React: A JavaScript library for building user interfaces.
Vite: A fast build tool for modern web projects.
Tailwind CSS: A utility-first CSS framework for rapid UI development.
Axios: A promise-based HTTP client for making API requests.
Firebase (Auth): Used for basic user authentication within the Canvas environment.
⚙️ Setup and Installation
Follow these steps to get a local copy of the project up and running on your machine.

Prerequisites
Node.js (LTS version recommended)
npm (Node Package Manager)
1. Clone the repository
Bash

git clone https://github.com/your-username/animal-explorer.git
cd animal-explorer
(Replace your-username/animal-explorer.git with your actual repository URL)

2. Install dependencies
Bash

npm install
3. Install Tailwind CSS dependencies
Bash

npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p
4. Configure Tailwind CSS
Open tailwind.config.js and ensure the content array includes your source files:

JavaScript

// tailwind.config.js
module.exports = {
  content: [
    "./index.html",
    "./src/**/*.{js,ts,jsx,tsx}",
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}
5. Add Tailwind Directives to your CSS
Open src/index.css (or src/App.css) and add the following:

CSS

/* src/index.css or src/App.css */
@tailwind base;
@tailwind components;
@tailwind utilities;
🔑 API Keys Configuration
This project relies on external APIs to fetch animal data. You need to obtain API keys and configure them:

API Ninjas (Animals API):
Go to https://api-ninjas.com/ and sign up for a free account to get your API key.
IUCN Red List API:
Go to https://api.iucnredlist.org/ and register to obtain your API token.
Once you have your keys, open src/components/AnimalSearch.jsx and replace the placeholder empty strings with your actual API keys:

JavaScript

// src/components/AnimalSearch.jsx
const API_NINJAS_KEY = 'YOUR_API_NINJAS_API_KEY'; // Replace with your API Ninjas key
const IUCN_API_KEY = 'YOUR_IUCN_REDLIST_API_KEY'; // Replace with your IUCN Red List key
▶️ Running the Project
After completing the setup and API key configuration, you can run the development server:

Bash

npm run dev
This will open the application in your browser (usually at http://localhost:5173/).
