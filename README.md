# murtala_shekoni_cinematch_prototype-
This directory contains a multi-page HTML version of the CineMatch application using vanilla JavaScript, HTML, and CSS.
# CineMatch - HTML Version

This directory contains a multi-page HTML version of the CineMatch application using vanilla JavaScript, HTML, and CSS.

## File Structure

```
├── pages/
│   ├── home.html           # Landing page with hero, trending, collections
│   ├── browse.html         # Browse with filters and sorting
│   ├── movie-details.html  # Individual movie details page
│   ├── watchlist.html      # User's saved movies
│   └── search.html         # Search functionality
├── public/
│   ├── styles.css          # All CSS styles
│   ├── data.js             # Movie data
│   └── utils.js            # Shared JavaScript utilities
└── index.html              # Single-page version (standalone)
```

## Pages

### 1. home.html
**Landing Page**
- Hero section with large search bar
- Trending movies grid (8 movies)
- Curated collections (4 collections)
- Browse by genre pills

### 2. browse.html  
**Browse/Explore Page**
- Left sidebar with filters:
  - Genre checkboxes
  - Decade checkboxes
  - Rating slider
- Active filter pills
- Sort dropdown (Popularity, Rating, Year, Title)
- Responsive movie grid
- Results count

### 3. movie-details.html
**Movie Details Page**
- Cinematic hero backdrop
- Movie poster (sticky on scroll)
- Action buttons (Add to Watchlist, Share, Watch Trailer)
- Quick info grid (Director, Cast, Budget, Box Office)
- Plot synopsis
- Cast & crew section
- Related movies grid

### 4. watchlist.html
**Watchlist Page**
- Empty state when no movies
- Stats dashboard (Total Movies, Total Runtime, Average Rating)
- Sort dropdown
- Clear All button with confirmation
- Movie grid with "Remove" buttons

### 5. search.html
**Search Results Page**
- Large search input
- Results count
- Movie grid
- No results state with suggestions
- Search by title, director, cast, or genre

## Features

### Shared Components
- **Header**: Sticky navigation with logo, Browse, Watchlist, Search
- **Footer**: Company info, quick links, legal links
- **Movie Card**: Reusable card with hover effects and watchlist toggle

### Functionality
- ✅ Watchlist management with localStorage persistence
- ✅ Filter by genre, decade, and minimum rating
- ✅ Sort by multiple criteria
- ✅ Search across all movie data
- ✅ Toast notifications
- ✅ Responsive design
- ✅ Smooth transitions and hover effects
- ✅ Back navigation support

### Data Storage
- Watchlist stored in localStorage
- 12 sample movies with complete metadata
- Persists across page reloads

## How to Use

### Option 1: Multi-Page Version
Navigate between pages using the header navigation or links:
- Start at `pages/home.html`
- Navigate to Browse, Watchlist, or Search
- Click movie cards to view details

### Option 2: Standalone Version
Open `index.html` directly for a single-page application experience with hash-based routing.

## Technologies Used
- **HTML5**: Semantic markup
- **CSS3**: Modern styling with CSS Grid, Flexbox, and animations
- **Vanilla JavaScript**: No frameworks or libraries
- **LocalStorage**: Client-side data persistence

## Browser Compatibility
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Responsive design supports desktop, tablet, and mobile

## Customization

### Adding More Movies
Edit `public/data.js` and add movie objects to the `movies` array.

### Styling
All styles are in `public/styles.css` with CSS custom properties for easy theming:
- `--primary`: Main brand color
- `--background`: Page background
- `--surface`: Card backgrounds
- `--text`: Primary text color
- `--text-muted`: Secondary text color

### Navigation
Links between pages use relative paths. Update paths in `public/utils.js` if changing directory structure.

## Notes
- All JavaScript is uncompiled vanilla JS
- No build process required
- No external dependencies
- Works offline once loaded
- Mobile-friendly responsive design

