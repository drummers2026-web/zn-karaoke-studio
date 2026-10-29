# ZN Karaoke Studio

A browser based karaoke player for iPhone, iPad, Android, and desktop. Add audio files from your device, create instrumental karaoke versions in the browser, adjust playback, sing along, and export the adjusted track.

## Use

1. Open `index.html` in a current browser.
2. Press **Try a demo** to load a short generated instrumental, or add your own audio file.
3. Press **Create karaoke**. On first use, the browser downloads the free karaoke separation model (about 30 MB). Processing time depends on your device.
4. Use tempo, pitch, backing volume, bass, treble, reverb, echo, and pan controls while singing.
5. Export the adjusted karaoke or demo as a WAV file with the download control.

Audio processing runs in your browser. Your song is not uploaded to this app's server. A connection is needed to download the separation model on first use.

## Hosting

The app is a static site. It can be hosted on GitHub Pages or another static web host. Microphone recording and some browser features require HTTPS. For development, serve the folder from a local web server rather than opening it with `file://` if a browser blocks file or microphone access.

## Limitations

Audio separation can leave some vocal sounds or remove parts of instruments. Results depend on the source mix and device performance. Playback tempo and pitch use the browser's playback-rate control. Vocal recording downloads the microphone recording separately; it does not yet mix a live vocal into the backing track.