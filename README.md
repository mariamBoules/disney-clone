# 🎬 Disney Clone – Movie Discovery App

This is a modern **Disney-style movie discovery app** built with **React**, **Vite**, **Tailwind CSS**, **TMDB API**, and **Appwrite**. Users can search through thousands of movies with a clean interface, responsive design, and real-time search analytics.

![hero](public/hero.png)

---

## 🚀 Features

- 🔍 **Search through 1000s of movies**
- ⚡ **Debounced input** for smooth searching
- 🧠 **Search term logging** using Appwrite database
- 🎨 **Responsive UI** styled with Tailwind CSS
- 🍿 **Popular movie discovery** when no search is active
- 🔁 **Real-time updates** using `useDebounce` and conditional fetches

---

## 🛠️ Tech Stack

- **Frontend**: React, Vite
- **Styling**: Tailwind CSS
- **APIs**:
  - [TMDB API](https://www.themoviedb.org/)
  - [Appwrite](https://appwrite.io/) (for search term tracking)

---

## 📦 Installation

1. **Clone the repo**

   ```bash
   git clone https://github.com/mariamBoules/disney-clone.git
   cd disney-clone
   ```

2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Add environment variables**

   Create a `.env` file in the root of the project:

   ```env
   VITE_TMDB_API_KEY=your_tmdb_api_key
   VITE_APPWRITE_PROJECT_ID=your_appwrite_project_id
   VITE_APPWRITE_DATABASE_ID=your_appwrite_database_id
   VITE_APPWRITE_COLLECTION_ID=your_appwrite_collection_id
   ```

4. **Run the development server**

   ```bash
   npm run dev
   ```

   Open [http://localhost:5173](http://localhost:5173) in your browser.

---

## 🧩 Folder Structure

```
├── public/
│   └── hero.png
├── src/
│   ├── Components/
│   │   ├── Search.jsx
│   │   ├── Spinner.jsx
│   │   └── MovieCard.jsx
│   ├── appwrite.js
│   └── App.jsx
├── .env
├── index.html
└── vite.config.js
```

---

## 📡 API Usage

- **TMDB** is used for fetching movies based on search queries or general popularity.
- **Appwrite** logs each unique search query and increments its count on repeat searches.

---

## ✨ Future Improvements

- 🔐 User authentication with Appwrite
- 💾 Save favorite movies
- 🌐 Deploy on Vercel or Netlify

---

## 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you'd like to change.

---

## 👩‍💻 Author

Made with ❤️ by [Mariam Boules](https://github.com/mariamBoules)
