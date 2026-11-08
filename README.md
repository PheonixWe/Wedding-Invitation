# Abhijith weds Kavya – wedding invitation

A single-page invitation: a Ganesh pop-up opens temple doors onto a film of the couple, with the Krishna flute music, a countdown, venue map and calendar buttons.

## Files (keep them together in the same folder)
- `index.html`  the invitation page
- `film.mp4`    background video (silent, loops)
- `poster.jpg`  still image shown while the video loads, and used for link previews
- `krishna_flute.mp3`  the music. It must have exactly this name and sit in the same folder as `index.html`; it starts playing when a guest taps **Open the invitation**

## Put it online with GitHub Pages
1. Sign in at github.com and click **New repository**. Name it, for example, `wedding`. Choose **Public**, then **Create repository**.
2. Click **uploading an existing file**, drag in `index.html`, `film.mp4`, `poster.jpg` and `krishna_flute.mp3`, then click **Commit changes**.
3. Open **Settings → Pages**. Under **Build and deployment**, set **Source** to **Deploy from a branch**, branch **main**, folder **/ (root)**, then **Save**.
4. After a minute or two your invitation is live at `https://YOUR-USERNAME.github.io/wedding/`. Send that link to your guests.

## Before you share it
- **WhatsApp RSVP:** open `index.html`, find `whatsapp: ""` near the bottom and add your number with country code, digits only (for example `"919876543210"`). Until you do, the RSVP section stays hidden.
- **Link preview image:** near the top of `index.html`, change `content="poster.jpg"` in the `og:image` line to the full address, for example `https://YOUR-USERNAME.github.io/wedding/poster.jpg`, so WhatsApp shows the picture when you share the link.
- **Calendar end times:** the reception (10:00 pm) and wedding (1:00 pm) end times are guesses. Edit `receptionCal` and `weddingCal` in the same place if you want different ones.

## About the music
- Phones and browsers only allow sound after a tap, so the music begins when the guest taps **Open the invitation**. A **Music** button stays on screen to turn it off and on.
- To use a different song, upload it as `krishna_flute.mp3` (same name) and replace the old file.
- If `krishna_flute.mp3` is missing, the page plays a built-in synthesised flute instead, so it is never silent.
