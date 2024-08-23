# edgetx-sound-pack

Includes Ardupilot flight modes. Uses elevenlabs.

## Setup

- install [bun](https://bun.sh)
- install ffmpeg
- install dependencies: `bun install`

## Usage

- Create an elevenlabs free account and get an API key, and create an env file: `cp example.env .env`
- Choose a voice on the elevenlabs website
- update script `index.ts` to use your preferred voice (`elevenlabsVoice` variable)
- run the script: `bun run index.ts`, which will generate sounds to `./sounds/$voice_name`
- move individual `.wav` files that you like to your `sdcard/SOUNDS` folder
- Use the sounds in your EdgeTX controller (Press SYS key, go to the "SPECIAL FUNCTIONS" page, and setup entries e.g. `SA- Ply Trk armed - []`)

## History

This project was created using `bun init` in bun v1.1.25. [Bun](https://bun.sh) is a fast all-in-one JavaScript runtime.
