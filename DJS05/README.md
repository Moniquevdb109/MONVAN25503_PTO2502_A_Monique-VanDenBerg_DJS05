# 🎙️ Podcast App — DJS05

A React podcast browsing app with dynamic routing, show detail pages, and season navigation.

## Getting Started
```bash
npm install
npm run dev
```

Then open `http://localhost:5173` in your browser.

## Features

- Browse all podcast shows with search, genre filter, and sort options
- Paginated results that adapt to screen size
- Click any show to view full details, seasons, and episodes
- Season switcher dropdown with episode list per season
- Filter and search state is preserved when navigating back from a detail page
- Loading and error states handled throughout

## Project Structure
```
src/
├── api/          # fetchData.js — all API calls
├── components/
│   ├── Filters/  # SearchBar, GenreFilter, SortSelect
│   ├── Podcasts/ # PodcastCard, PodcastGrid, PodcastDetail
│   └── UI/       # Header, Loading, Error, Pagination, GenreTags
├── context/      # PodcastContext — global state
├── data/         # Static genre ID → title mapping
├── pages/        # Home, ShowDetail
├── styles/       # All CSS modules
└── utils/        # formatDate
```

## API

Data sourced from `https://podcast-api.netlify.app`
