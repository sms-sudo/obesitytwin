Obesity Treatment Twin: the web tool

What it is
  The deployed digital twin, fitted on every course of treatment at MGB from 2018 to August 2025, running in a web
  browser. A clinician enters what they know about one patient; the page shows the expected course of weight under ten
  strategies with its 80% range and the chance of each amount of loss, the change in six cardiometabolic measures at
  12 months, and the two-year risk of 20 complications. At a later visit it updates the forecast from the weights
  measured since the start, whether the patient is taking the medicine and the dose reached.

What is in this folder
  index.html   the page (plain HTML and JavaScript, no external libraries; fonts from Google Fonts if online)
  models/      89 model files (decision trees: splits and leaf values only, no patient data or counts; every leaf
               rests on at least 25 patients) and twin_spec.json, which says how they fit together

How to open it
  Browsers do not let a page read files from a folder opened directly, so serve the folder:
    1. Open a terminal in this folder.
    2. Run:  python -m http.server 8000
    3. Open http://localhost:8000 in a browser.
  Nothing a user enters leaves the browser.

Sharing
  The models were learned from MGB records. Share the tool outside MGB only after MGB's approval for release of
  the model files.
