# Twimba

A small Twitter-like demo app built with Vite. Post tweets, like, retweet and view replies.

## Quick start

1. Install dependencies:

```sh
npm install
```

2. Run the dev server:

```sh
npm run dev
```

Open the app in your browser (Vite default port, e.g. <http://localhost:5173>).

See scripts in [package.json](package.json).

## Files

- Main HTML: [index.html](index.html)  
- App logic: [index.js](index.js) — UI event handlers and rendering (see [`handleLikeClick`](index.js), [`handleRetweetClick`](index.js), [`handleReplyClick`](index.js), [`handleTweetBtnClick`](index.js), [`getFeedHtml`](index.js), [`render`](index.js)).  
- Tweets data: [`tweetsData`](data.js) in [data.js](data.js).  
- Styles: [index.css](index.css)  
- Vite config: [vite.config.js](vite.config.js)  
- Static assets: [images/](images/)

## Features

- Render a feed from [`tweetsData`](data.js).  
- Like and retweet toggles handled by [`handleLikeClick`](index.js) and [`handleRetweetClick`](index.js).  
- Show/hide replies via [`handleReplyClick`](index.js).  
- Create new tweets with [`handleTweetBtnClick`](index.js) (uses `uuid` from a CDN).

## Notes

- The project uses Vite ([vite](package.json)).  
- Tweet objects are stored in-memory in [`tweetsData`](data.js); no backend persistence.  
- Profile images and icons live in [images/](images/).

## License

MIT
