# Saint Rose Property Assessments

Interactive web application for browsing and comparing 69 former College of Saint Rose properties in Albany, NY.

## Features

- **Property Grid** — Browse all 69 properties with photos, condition scores, and investment risk ratings
- **Search & Filter** — Find properties by address or building name; filter by risk level; sort by score, size, or address
- **Property Detail View** — Full condition ratings across 9 assessment categories and up to 58 building systems per property
- **Photo & Floor Plan Gallery** — View extracted assessment photos and architectural floor plans
- **Property Comparison** — Compare up to 5 properties side-by-side across every system rating
- **External Links** — Direct links to Google Maps, Street View, and Albany Tax Assessment for each property

## Data Source

Data extracted from official Building Condition Assessment reports covering the former College of Saint Rose campus properties, acquired by the Albany Pine Hills Land Authority.

- **69 properties** assessed
- **3,938 individual system ratings** across 9 categories
- **Rating scale**: 1 (Critical) to 5 (Excellent)
- **Investment Risk Tiers**: Low (4.0-5.0), Moderate (3.0-3.9), High (2.5-2.9), Very High (below 2.5)

## Deployment

This is a static site — no server or build step required.

### GitHub Pages

1. Push this repository to GitHub
2. Go to **Settings → Pages**
3. Set source to **Deploy from a branch**
4. Select **main** branch, root folder
5. Your site will be live at `https://yourusername.github.io/saint-rose-properties/`

### Any Static Host

Upload all files to any static hosting service (Netlify, Vercel, etc.)

## File Structure

```
├── index.html          # Main application (React SPA)
├── data.js             # Property data (69 properties, embedded JSON)
├── images/             # Optimized property photos and floor plans
│   ├── 1000_Madison_Avenue/
│   ├── 1001_Madison_Avenue/
│   └── ...             (69 property folders, 243 images total)
└── README.md
```

## Technology

- React 18 (CDN)
- Vanilla CSS (no framework dependencies)
- All data embedded client-side (no API required)
- Fully responsive design
