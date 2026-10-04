# For Nuzra, With Love

A complete, mobile-friendly birthday website. The HTML, styles, JavaScript, photos, videos, and instrumental MP3 are all included in this folder. No build step or package installation is needed.

## Open it in VS Code

1. Extract `Nuzra-Birthday-VSCode.zip`.
2. In VS Code, choose **File → Open Folder** and select the extracted `nuzra-birthday` folder.
3. Open `index.html` in a browser. You can also use the optional **Live Server** extension in VS Code for a local preview.

For hosting, publish the contents of the extracted `nuzra-birthday` folder together. Do not upload only the three code files: the site needs the complete `assets` folder. Keep the media folders and filenames exactly as they are; hosted servers distinguish uppercase and lowercase filenames.

## Main files

- `index.html` — the page structure and sections.
- `styles.css` — colors, layout, responsive styles, and animations.
- `script.js` — gallery, video, birthday music, wish button, and page interactions.
- `assets/images/` — the photos used by the page.
- `assets/videos/new-first/video-01.mp4` through `video-07.mp4` — your seven new clips, in the order you provided. They appear first in the video gallery.
- `assets/videos/video-01.mp4` through `video-09.mp4` — the original nine clips, shown after the new seven.
- `assets/audio/happy-birthday-instrumental.mp3` — the instrumental, set to repeat. It pauses while a video plays with sound.

Keep the `assets` folder beside the three main files so all media paths continue to work. The page attempts to start the looping birthday song on open. Browsers that block sound autoplay will start it on the first page tap or click; videos stay paused while the song is playing. If a hosted video fails to load, check that the matching MP4 is present in `assets/videos/`; the video caption will also show a hosting hint.

The quote typewriter and photo gallery start only when their sections enter view. The photo gallery begins with photo 01.

## Personalize it

The `birthdayConfig` object near the top of `script.js` contains the name, captions, birthday wishes, reasons, and media paths. The photo gallery uses `assets/images/nuzra/photo-01.jpeg` through `photo-29.jpeg`; the video gallery lists the seven clips in `assets/videos/new-first/` first, followed by the original nine clips in `assets/videos/`.

