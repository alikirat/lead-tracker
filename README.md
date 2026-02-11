# Lead Tracker Chrome Extension

A simple Chrome extension for saving and managing leads (URLs). Keep track of interesting websites, resources, or potential business leads with easy-to-use buttons and persistent storage.

## Features

- **Save Input**: Manually enter and save any URL or text lead
- **Save Tab**: Capture the current active tab's URL with one click
- **Delete Last**: Remove the most recently added lead
- **Delete All**: Clear all saved leads (double-click for safety)
- **Persistent Storage**: All leads are saved in localStorage and survive browser restarts
- **Clickable Links**: All saved URLs are displayed as clickable links that open in new tabs

## Installation

1. Clone or download this repository
2. Open Chrome and navigate to `chrome://extensions/`
3. Enable "Developer mode" (toggle in top-right corner)
4. Click "Load unpacked"
5. Select the `lead-tracker` folder
6. The extension icon will appear in your Chrome toolbar

## Usage

1. Click the extension icon in your Chrome toolbar to open the popup
2. **To save a URL manually**: Type or paste it in the input field and click "SAVE INPUT"
3. **To save the current tab**: Click "SAVE TAB" button
4. **To delete the last lead**: Click "DELETE" button
5. **To clear all leads**: Double-click "DELETE ALL" button
6. Click any saved lead to open it in a new tab

## File Structure

```
lead-tracker/
├── index.html      # Extension popup interface
├── index.css       # Styling for the popup
├── index.js        # Main functionality and event handlers
├── manifest.json   # Chrome extension configuration
└── README.md       # This file
```

## Technical Details

- **Manifest Version**: 3 (latest Chrome extension format)
- **Permissions**: Tabs (required for capturing active tab URL)
- **Storage**: localStorage API for data persistence
- **Browser Compatibility**: Chrome (Manifest V3)