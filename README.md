# GA4 BigQuery Project ID Discovery Tool

This tool helps you find all BigQuery project numbers associated with your GA4 properties. It shows which GA4 properties have BigQuery exports enabled and their corresponding project numbers.

## Check if Python is Already Installed

### Windows:
1. Press Windows key + R
2. Type `cmd` and press Enter
3. In the black window that appears, type: `python --version`
4. If you see a response like `Python 3.x.x`:
   - Python is already installed
   - Skip to "Download the Tool" section
5. If you see `'python' is not recognized`:
   - Python is not installed
   - Continue with "Install Python" section

### Mac:
1. Press Command + Space
2. Type "Terminal" and press Enter
3. In the window that appears, type: `python3 --version`
4. If you see a response like `Python 3.x.x`:
   - Python is already installed
   - Skip to "Download the Tool" section
5. If you see `command not found`:
   - Python is not installed
   - Continue with "Install Python" section

## Setup Instructions

### 1. Install Python (only if not already installed)
1. Go to [Python Downloads](https://www.python.org/downloads/)
2. Download the latest version for your system:
   - **Windows**: Click "Download Python 3.x.x"
   - **Mac**: Click "Download Python 3.x.x for macOS"
3. Install Python:
   - **Windows**: 
     - Double-click the downloaded file (usually starts with "python")
     - Check ✅ "Add Python to PATH" box at the bottom ⚠️ Very Important!
     - Click "Install Now"
     - Wait for the installation to complete
     - Click "Close" when finished
     - Restart your computer
   - **Mac**: 
     - Double-click the downloaded file (ends in .pkg)
     - Click "Continue" through the installation screens
     - Click "Install" (you may need to enter your Mac password)
     - Click "Close" when finished

4. Verify Installation:
   - Follow the "Check if Python is Already Installed" steps above
   - You should now see a Python version number
   - If not, restart your computer and try again

### 2. Start the Tool
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
4. Drag your tool folder (the one you downloaded and unzipped from Slack) onto the Terminal window
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

## Need Help?
Contact [YOUR_ADMIN_NAME] at [YOUR_ADMIN_EMAIL]
