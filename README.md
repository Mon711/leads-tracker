# Leads Tracker

Leads Tracker is a small Chrome extension that lets you save useful links in one place.

You can:

- save a URL by typing it into the input field
- save the current browser tab with one click
- view saved leads as clickable links
- clear all saved leads from local storage

## Project Files

- `index.html` - popup layout for the extension
- `index.css` - popup styling
- `index.js` - app logic for saving, rendering, and deleting leads
- `manifest.json` - Chrome extension configuration
- `icon.png` - extension icon

## How It Works

The app stores leads in the browser using `localStorage`.

- On load, it reads saved leads from `localStorage`
- When you click `SAVE INPUT`, it stores the typed value
- When you click `SAVE TAB`, it stores the URL of the current tab
- When you double-click `DELETE ALL`, it clears saved leads

## How To Run

1. Open Chrome and go to `chrome://extensions/`
2. Turn on **Developer mode**
3. Click **Load unpacked**
4. Select this project folder
5. Open the extension from the Chrome toolbar

## Permissions

This extension uses the `tabs` permission so it can read the URL of the active tab when you click `SAVE TAB`.

## Notes

- Saved leads stay available because they are stored in browser local storage
- `DELETE ALL` works on double-click, not single click
