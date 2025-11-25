# fuzbal

A simple web app for tracking football league standings and match history.

## Features

- ✅ Add players
- ✅ Record matches (select winners/losers)
- ✅ Automatic standings calculation
- ✅ Match history tracking
- ✅ Win/loss statistics and form tracking
- ✅ All data stored locally in browser (localStorage)

## How to Use

1. **Add Players**: Click the users icon (👥) in the header to add players
2. **Record a Match**: Click the green + button at the bottom right
   - Select up to 5 winners
   - Remaining players are automatically assigned as losers
   - All players must be assigned to either winners or losers
3. **View Standings**: See player rankings, win/loss records, and recent form
4. **View History**: Browse past matches

## Hosting Options

Since this is a single HTML file with no backend, you can host it anywhere that serves static files:

### Option 1: GitHub Pages (Free & Easy)
1. Create a GitHub repository
2. Upload `main.html` (rename it to `index.html` for GitHub Pages)
3. Go to repository Settings → Pages
4. Select main branch and save
5. Your app will be live at `https://yourusername.github.io/repository-name`

### Option 2: Netlify (Free & Easy)
1. Go to [netlify.com](https://netlify.com)
2. Drag and drop your `main.html` file (or connect GitHub repo)
3. Done! You get a free URL instantly

### Option 3: Vercel (Free & Easy)
1. Go to [vercel.com](https://vercel.com)
2. Import your project or drag and drop `main.html`
3. Deploy instantly

### Option 4: Any Static Hosting
- Cloudflare Pages
- Firebase Hosting
- AWS S3 + CloudFront
- Any web server that can serve HTML files

## Data Storage

All data is stored in the browser's localStorage. This means:
- ✅ No database needed
- ✅ Works offline
- ⚠️ Data is browser-specific (each user has their own data)
- ⚠️ Clearing browser data will delete all records

## Technical Details

- Pure HTML/CSS/JavaScript
- React 18 (via CDN)
- Tailwind CSS (via CDN)
- No build process required
- Single file application

