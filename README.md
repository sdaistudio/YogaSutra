# Yoga Sutras for Young Minds

Patanjali's 195 Yoga Sutras retold for children (around age 10), with an animated picture for every sutra, word-by-word meanings and Sanskrit read-aloud. Based on Swami Vivekananda's translation and commentary.

- **Samadhi Pada**: 51 sutras
- **Sadhana Pada**: 55 sutras
- **Vibhuti Pada**: 56 sutras
- **Kaivalya Pada**: 33 sutras (numbered as in Swami Vivekananda's edition, which has no separate 4.16)

The whole site is one file, `index.html`. It needs no build step and no server code.

## Put it on GitHub Pages

1. Create a new repository on GitHub, for example `yoga-sutras`.
2. Upload `index.html` and this `README.md`: **Add file → Upload files**, then **Commit**.
3. Open **Settings → Pages**. Under **Build and deployment**, set Source to **Deploy from a branch**, Branch to **main**, and folder to **/ (root)**. Click **Save**.
4. After a minute or two the site is live at `https://<your-username>.github.io/yoga-sutras/`.

## Links to a single sutra

- A Pada: `…/#p2`
- A sutra: `…/#s2-46` (Pada 2, Sutra 46)

## Sanskrit audio

By default the **Listen** buttons use the visitor's own device voice. It uses a Hindi voice when one is installed; Chrome and Edge include one.

To use proper recordings instead, for example a teacher chanting:

1. Record each sutra as an MP3.
2. Name each file `<pada>-<sutra>.mp3`, for example `1-1.mp3`, `1-2.mp3` … `4-33.mp3`.
3. Put the files in a folder called `audio` next to `index.html`, and upload that folder to the repository.

When a recording exists, **Whole sutra** and **Slowly** play it. When it does not, the site falls back to the device voice automatically, so you can add recordings a few at a time. **Word by word** always uses the device voice.

## Editing the content

All sutra text lives in `index.html`, inside `const SUTRAS=[ … ]`. Each sutra is one entry:

| field | what it is |
|---|---|
| `p`, `n` | Pada and sutra number |
| `skt`, `tr` | Sanskrit (Devanagari) and transliteration |
| `sw` | Swami Vivekananda's translation (verbatim) |
| `title`, `line` | card title and one-line summary |
| `words` | word-by-word meanings: `[Sanskrit, roman, meaning]` |
| `kid` | the simple-words explanation (1–2 paragraphs) |
| `quote` | a verbatim line from Swamiji's commentary, or `null` |
| `note`, `think` | optional note and the "Think about it" question |
| `motif` | which animated picture to show (eye, lake, flame, lotus…) |

Edit the text in any editor, then upload the file again.

## Source

Text follows *Patanjali Yoga Sutras: Sanskrit text with transliteration, translation and commentary* by Swami Vivekananda. Lines in quotation marks are Swamiji's own words. Everything else is a simplified retelling for young readers.
