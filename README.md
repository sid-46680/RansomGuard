# RansomGuard — Ransomware Detection & Response Lab

A browser-based educational cybersecurity lab demonstrating explainable file triage, synthetic ransomware-like behavior monitoring, and incident response planning.

## Features
- **Local file scan:** analyzes up to the first 2 MiB of a user-selected file, without uploading it.
- **Entropy heatmap:** visualizes Shannon entropy across file blocks.
- **File indicators:** checks known headers, suspicious extensions, ransom-note language, and mixed-entropy patterns.
- **Behavior monitor (simulation):** replays normal office activity or a synthetic ransomware-like burst, including a simulated canary event and containment alert.
- **Blast-radius simulator:** models the effect of response delay on potentially affected files.
- **Response checklist:** provides educational incident response guidance.

## Run locally
No installation or dependencies are required. Open `index.html` in a modern web browser. An internet connection is optional for the application logic; Google Fonts may load when online.

Alternatively, start a local server:

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000/.

## GitHub Pages
1. Push the repository to GitHub.
2. Go to **Settings → Pages**.
3. Select **Deploy from a branch**, branch `main`, folder `/ (root)`.
4. Save and wait for GitHub Pages to publish the site.

## Safety and limitations
This is **not** a production antivirus or endpoint detection product. Browser pages cannot monitor arbitrary system file changes or isolate processes. The behavior-monitor and containment features are simulations. File scanning is heuristic and may generate false positives or miss threats. Never rely on this demonstration to establish that a file is safe.

No real malware samples are necessary for demonstrations. Do not publish sensitive documents, incident evidence, secrets, or malware binaries in the repository.

## Technology
HTML5, CSS3, vanilla JavaScript, Browser File API, SVG.

## Project structure
```
RansomGuard/
├── index.html
├── README.md
├── .gitignore
└── LICENSE
```

## License
See `LICENSE`. Replace the copyright placeholder with the appropriate copyright holder before publishing.
