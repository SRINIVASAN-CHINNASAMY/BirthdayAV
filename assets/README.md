# Adding your photos and music

Drop your files into the two folders here, using these **exact filenames**
(or edit the matching path inside the `CONFIG` object near the top of
`index.html`'s `<script>` if you'd rather use your own names).

## assets/images/
| Filename | Used for |
|---|---|
| `photo-01.jpg` … `photo-10.jpg` | The 10 photos in the "Memory Lane" gallery |
| `gate-background.jpg` *(optional)* | Full background image on the very first "ask a friend's name" page |
| `finale-background.jpg` *(optional)* | Full background image on the last "Happy Birthday" page |

- Any of the 10 gallery photos can be skipped — just leave that slot's caption as "Add a photo" or remove that entry from `CONFIG.photos`.
- `.jpg`, `.png`, and `.webp` all work. If you use a different extension, update the filename in `CONFIG.photos` / `CONFIG.pageBackgrounds` to match.
- Keep photos reasonably sized (under ~2–3 MB each) so the page loads quickly.

## assets/audio/
| Filename | Used for |
|---|---|
| `gallery-music.mp3` | Plays quietly under the photo gallery |
| `our-song.mp3` | The track on the dedicated "Our Song" page |
| `background-music.mp3` *(optional)* | Whole-site background music toggle (top-left button) — leave this file out and leave `CONFIG.backgroundMusicSrc` blank to hide that button entirely |

- MP3 is the safest format for browser compatibility.
- These are normal files sitting in your GitHub repo — no Google Drive, no special sharing settings, no CORS/CORB issues.

## After adding files
Just commit and push the `assets/` folder (with your files inside) alongside
`index.html` to your GitHub repo. Nothing else needs to change — the
filenames already match what `CONFIG` in `index.html` expects.
