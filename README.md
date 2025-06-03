# 🐾 Animal Explorer

A simple and beautiful web application built with **React** and **Tailwind CSS** to explore information about various animals, including their **biological names**, **characteristics**, and **conservation status**.

---

## ✨ Features

* 🔍 **Animal Search**: Search for animals by their common names.
* 📚 **Detailed Information**: View scientific names, diet, habitat, lifespan, and more.
* 🌍 **Conservation Status**: Get IUCN Red List conservation status.
* 📱 **Responsive Design**: Clean and modern interface that looks great on all devices.
* 🔗 **API Integration**: Fetches data from external APIs for comprehensive and accurate information.

---

## 🚀 Technologies Used

* **React** – Frontend library for building user interfaces.
* **Vite** – Next-generation frontend tooling.
* **Tailwind CSS** – Utility-first CSS framework for fast and elegant styling.
* **Axios** – Promise-based HTTP client for API requests.
* **Firebase (Auth)** – User authentication (optional, for extended features).

---

## ⚙️ Setup and Installation

### ✅ Prerequisites

* Node.js (LTS version recommended)
* npm (Node Package Manager)

### 📦 1. Clone the Repository

```bash
git clone https://github.com/your-username/animal-explorer.git
cd animal-explorer
```

> Replace `your-username` with your GitHub username.

### 📅 2. Install Dependencies

```bash
npm install
```

### 🌝 3. Install Tailwind CSS Dependencies

```bash
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p
```

### ⚙️ 4. Configure Tailwind CSS

Update `tailwind.config.js`:

```js
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
```

### 🎨 5. Add Tailwind Directives to CSS

In `src/index.css` (or `src/App.css`):

```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

---

## 🔑 API Keys Configuration

This project uses external APIs. You'll need API keys:

### 🐾 API Ninjas (Animals API)

* Sign up at: [https://api-ninjas.com/](https://api-ninjas.com/)
* Obtain your **Animals API key**

### 🌿 IUCN Red List API

* Register at: [https://apiv3.iucnredlist.org/](https://apiv3.iucnredlist.org/)
* Obtain your **IUCN Red List API token**

### 🔧 Add Your API Keys

In `src/components/AnimalSearch.jsx`, replace placeholders with your actual keys:

```js
const API_NINJAS_KEY = 'YOUR_API_NINJAS_API_KEY'; // Replace with your API Ninjas key
const IUCN_API_KEY = 'YOUR_IUCN_REDLIST_API_KEY'; // Replace with your IUCN Red List key
```

---

## ▶️ Running the Project

Once setup is complete, start the development server:

```bash
npm run dev
```

Then open your browser and navigate to:

```
http://localhost:5173/
```

---

## 🙌 Contributing

Contributions are welcome! Please fork the repository and submit a pull request.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 📬 Contact

Created with ❤️ by [Your Name](https://github.com/your-username)

---
