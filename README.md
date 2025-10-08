# Tic-Tac-Toe Game

This is a small Tic-Tac-Toe web game. The project has been updated to support Progressive Web App (PWA) installation and basic offline support via a service worker.

How to test locally

- Serve the folder over HTTP (required for service workers). A quick command using Python (from the project folder):

```sh
# Windows (cmd.exe)
python -m http.server 8000
```

- Open http://localhost:8000 in Chrome or Edge. Open DevTools > Application to inspect the service worker and manifest. Use the "Install" option in the address bar or browser menu to install as a PWA.

Notes

- The service worker caches the app shell (HTML/CSS/JS) so the game can be launched offline after the first load.
- If you deploy to a subpath, adjust `start_url` in `manifest.json` and the service worker scope as needed.
"# lab-task-5" 
