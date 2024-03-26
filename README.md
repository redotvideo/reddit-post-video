# Create Short Videos from Reddit Posts 🪄

This project uses [Revideo](https://github.com/redotvideo/revideo) to automatically generate short videos from Reddit Post urls. Here is a (low resolution) example:

https://github.com/redotvideo/reddit-post-video/assets/122226645/0489e6b9-2b49-4717-b4d7-e94a909cbf40

Two code files do most of the heavy lifting for this project:

- `src/renderScript.ts` is a node process that fetches the contents of the provided Reddit post url, generates a voiceover using [ElevenLabs](https://elevenlabs.io/), gets timestamps for the voiceover and organizes all of this metadata in `./metadata.json`. Finally, it calls `renderVideo` to render & export the project using a headless browser.
- `src/scenes/example.tsx` defines the animation flow and audio of our video

  ## Getting Started

  First, you should clone the repository and install all dependencies:

   ```bash
   git clone https://github.com/redotvideo/reddit-post-video.git
   cd reddit-post-video
   npm install
   ```

   You can now look at the example project using the editor:

  ```bash
  npm start
  ```
