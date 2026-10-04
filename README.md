# ArSL Recognition: browser demo

Recognizes the 32 static hand shapes of the Arabic Sign Language alphabet from your
webcam, one letter at a time, and builds words from them.

**Try it:** https://anas-71.github.io/arsl-demo/

- Runs entirely in your browser: the camera video is never uploaded or stored.
- Hand tracking by [MediaPipe](https://github.com/google-ai-edge/mediapipe); a small
  classifier trained on hand landmarks names the letter, or says "not recognized".
- How it works and dataset credits: see the site's About page (`about.html`).

## Run it locally

Serve this folder with any static web server, then open the address it prints,
for example `npx serve .`. Opening `index.html` directly from disk does not work
(browsers block the camera and JavaScript modules on `file://` pages).

## Licences

- Trained model (`model/model.json`): CC BY-SA 4.0, as it is trained in part on the
  AASL dataset (CC BY-SA 4.0). Other training data: ArSL21L (CC BY 4.0).
- Reference images (`reference/`): from the ArASL2018 dataset's chart (CC BY 4.0).
- MediaPipe files (`mediapipe/`): Apache License 2.0, see `mediapipe/LICENSE`.
