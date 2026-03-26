# Flutter Web Build

## What's Inside

This folder contains a complete Flutter Web release build with:

- Compiled Dart code (JavaScript)
- Assets (images, fonts, etc.)
- `index.html` entry point
- Required Flutter framework files

## Running Locally

Opening `index.html` in browser is not sufficient to locally run Flutter Web App. To run Flutter Web App it needs needs to be locally hosted by HTTP server. All commands have to be run from folder with `index.html` file.

### Example 1: Python HTTP Server

 Start a local server (Python 3):
 
```bash
python3 -m http.server 8000
```

Open `http://localhost:8000` in your browser.

### Example 2: Node.js HTTP Server

Install serve globally (one-time):

```bash
npm install -g serve
```

Start the server:

```bash
serve -s . -l 8000
```

## Deploying to Production

For information about deploying your app [see official documentation](https://docs.flutter.dev/deployment/web#deploying-to-the-web)

If your app is hosted at a subdirectory (e.g., `example.com/myapp/`), ensure that `<base href="/">` in `index.html` is properly set. Otherwise, assets may fail to load.
