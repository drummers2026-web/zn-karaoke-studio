# ZN Karaoke Studio

A browser based karaoke player for iPhone, iPad, Android, and desktop. The header features the Zubair Naina Music Hub logo and a warm black-and-gold theme. Add audio files from your device, create instrumental karaoke versions in the browser, adjust playback, sing along, and export the adjusted track.

## Use

Use the **Player** page to play, adjust, loop, and record. Open **Karaoke Creator** to make an instrumental. The two views share the same player session, so switching pages keeps your current track loaded.

1. Open `index.html` in a current browser.
2. Press **Try a demo** to load a short generated instrumental, or add your own audio file.
3. Open **Karaoke Creator**, then choose a song. The app estimates its approximate Western major/minor key on your device and shows the result; you can set the Player key manually. This estimate is only a guide and does not identify an Indian raga.
4. Press **Create karaoke**. On first use, the browser downloads the free karaoke separation model (about 30 MB). Processing time depends on your device. Phones may take several minutes; keep the page open and the screen awake until it finishes.
5. Choose a target key to transpose the song; otherwise use the pitch slider. Use tempo, backing volume, bass, treble, reverb, echo, and pan controls while singing.
6. Set loop points A and B to repeat a section for practice. Press the red record control for a three-second count-in, then record your voice with the adjusted backing; stop to review your voice and backing in the built-in player, then download the take if you like it.
7. Load lyrics by pasting text or choosing a .txt file. Timed .lrc files follow playback automatically; plain text can be read and scrolled while singing.

Track-specific adjustment settings are saved in this browser on this device. Audio processing and the approximate key estimate run in your browser. Your song is not uploaded to this app's server. A connection is needed to download the separation model on first use. Key estimates can be inaccurate for dense mixes, songs that change key, or Indian classical music. The app does not detect ragas; raga identification requires more than matching a Western major/minor scale.

## Hosting

The app is a static site. It can be hosted on GitHub Pages or another static web host. Microphone recording and some browser features require HTTPS. For development, serve the folder from a local web server rather than opening it with `file://` if a browser blocks file or microphone access.

## Limitations

Audio separation can leave some vocal sounds or remove parts of instruments. Results depend on the source mix and device performance. Playback tempo and pitch use the browser's playback-rate control. Performance recording mixes the microphone with the adjusted backing track and downloads a recording. Plain-text lyrics are not automatically timed; use an .lrc file with timestamps for synchronized highlighting.

## Logo asset

Keep zn-music-hub-logo.webp beside index.html when hosting the site; the header loads it directly.


## Install icon and name

The install name is ZN Karaoke Studio. Keep icon-full-192.png and icon-full-512.png beside index.html and manifest.webmanifest so browsers can use the complete ZN Music Hub logo for the installed app icon.


## iPhone and iPad installation

Open the site in Safari, tap Share, choose Add to Home Screen, enable Open as Web App if shown, and tap Add. If the option is hidden, scroll the Share menu or use Edit Actions to add it.


## Suggestions and feedback

The suggestion form asks for the visitor name, email, and message, then opens their email app addressed to drummers2026@gmail.com. The visitor reviews and sends the email from their own app.
