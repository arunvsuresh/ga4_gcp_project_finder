# GA4 BigQuery Project ID Discovery Tool

This tool helps you find all BigQuery project numbers associated with your GA4 properties. It shows which GA4 properties have BigQuery exports enabled and their corresponding project numbers.

## Setup Instructions

### 1. Install Python (if you don't already have it)
1. Go to [Python Downloads](https://www.python.org/downloads/)
2. Download the latest version for your system:
   - **Windows**: Click "Download Python 3.x.x"
   - **Mac**: Click "Download Python 3.x.x for macOS"
3. Install Python:
   - **Windows**: 
     - Run the downloaded file
     - Check "Add Python to PATH" ⚠️ Important!
     - Click "Install Now"
   - **Mac**: 
     - Open the downloaded file
     - Follow installation prompts

### 2. Download the Tool
1. Download these files:
   - `index.html`
   - `config.js` (contains authentication credentials)
2. Put both files in a new folder on your computer
   - Example folder location: `Documents/ga4-tool`

### 3. Start the Tool
#### Windows:
1. Press Windows key + R
2. Type `cmd` and press Enter
3. Type `cd ` (including the space)
4. Drag your tool folder onto the Command Prompt window
5. Press Enter
6. Type: `python -m http.server 8000`
7. Keep this window open

#### Mac:
1. Press Command + Space
2. Type "Terminal" and press Enter
3. Type `cd ` (including the space)
4. Drag your tool folder onto the Terminal window
5. Press Enter
6. Type: `python -m http.server 8000`
7. Keep this window open

### 4. Use the Tool
1. Open Chrome or Firefox
2. Go to: http://localhost:8000
3. Click "Sign in with Google"
4. Use your work Google account
5. Select GA4 accounts to analyze
6. Click "Get Project IDs"

### 5. Stop the Tool
When finished:
1. Go back to Command Prompt/Terminal
2. Press Ctrl + C (Windows) or Command + C (Mac)
3. Close the window

## Troubleshooting

### "python is not recognized"
Try:
```
python3 -m http.server 8000
```

### "port 8000 is in use"
Try:
```
python -m http.server 8080
```
Then use http://localhost:8080 in your browser

### Authentication Failed
1. Make sure you're using your work Google account
2. Contact your admin for help

### Nothing happens when clicking "Sign in"
1. Make sure both `index.html` and `config.js` are in the same folder
2. Check with your admin that you have the correct `config.js`
