# 📰 DailyNews - React News Application

## 📌 Overview
**DailyNews** is a modern real-time news web application built using **ReactJS**. It fetches the latest articles from [NewsAPI.org](https://newsapi.org/) and displays them based on user-selected categories. The app is designed for a smooth and responsive experience, supporting **infinite scrolling**, **lazy loading**, and performance optimizations using **React memoization techniques**.

---

## 🚀 Features

- 🔍 Real-time news fetching via **RESTful API**
- 📚 Category-based filtering (Technology, Business, Sports, etc.)
- 🔁 **Infinite scrolling** for seamless content loading
- 💤 **Lazy loading** of images to boost performance
- ⚡ Optimized re-renders with **React.memo**, `useMemo`, and `useCallback`
- 💬 Error handling for failed API requests
- 📱 Responsive design for desktop and mobile
- 💡 Clean and reusable components like `NewsList`, `NewsCard`, `Navbar`

---

## 🛠️ Tech Stack

- **Frontend:** ReactJS, JSX, CSS
- **State Management:** React Hooks (`useState`, `useEffect`)
- **APIs:** [NewsAPI.org](https://newsapi.org/)
- **Build Tool:** Vite or Create React App (based on your setup)
- **Deployment:** (Optional) Netlify / Vercel / GitHub Pages

---

## 🧠 How It Works

1. The app initializes using the `App` component.
2. News articles are fetched using `fetch()` in the `useEffect()` hook.
3. Articles are stored in a state variable using `useState`.
4. The `map()` function renders each article dynamically via the `NewsCard` component.
5. Category selection updates the API endpoint to fetch relevant data.
6. Infinite scroll triggers more API calls as the user scrolls to the bottom.
7. Lazy loading improves performance by loading images only when visible.

---

## 📂 Folder Structure
DailyNews/ ├── public/ ├── src/ │ ├── components/ │ │ ├── Navbar.js │ │ ├── NewsCard.js │ │ └── NewsList.js │ ├── App.js │ ├── index.js │ └── App.css ├── .env └── README.md

---

## ⚙️ Installation & Usage

```bash
# Clone the repo
git clone https://github.com/your-username/DailyNews.git

# Navigate to the folder
cd DailyNews

# Install dependencies
npm install

# Add your API key to .env
REACT_APP_NEWS_API_KEY=your_api_key_here

# Start the development server
npm start
