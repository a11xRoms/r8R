# r8R

A modern YouTube-style static video platform made for GitHub Pages.

## Included
- Responsive dark + blue UI
- Video upload from the browser
- Title, description, hashtags, thumbnail, visibility and category
- Video player
- Search
- Home / Trending / Subscriptions / Library / History / Liked / Playlists navigation
- Likes
- Subscriptions
- Comments
- Share button
- Delete your own uploads
- Profile page
- Settings and light/dark theme
- Browser persistence with IndexedDB + localStorage

## GitHub Pages limitation

GitHub Pages is static hosting. It cannot provide a real shared server/database for public uploads. This version therefore stores uploaded video files **locally in the viewer's browser** using IndexedDB. That makes the upload and playback features actually work on GitHub Pages, but a video uploaded by one person will not appear for another person.

For a real multi-user r8R service, connect the same frontend to a backend/storage service such as Cloudflare R2/Supabase/Firebase/AWS S3 and add authentication.

## Deploy

1. Put `index.html`, `style.css`, and `app.js` in your GitHub repository.
2. Open **Settings → Pages**.
3. Choose **Deploy from a branch** and select the branch/folder containing these files.
4. Open the generated GitHub Pages URL.

No build step is required.
