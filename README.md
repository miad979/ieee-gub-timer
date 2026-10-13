# IEEE GUB SB Countdown Timer

A premium-looking, single-page countdown timer for events organised by the IEEE GUB Student Branch at Green University of Bangladesh (GUB). It is one self-contained `index.html` file with no build step and no dependencies.

## Features

- Logo layout: GUB (top left), IEEE GUB Student Branch (top right), IEEE Computer Society and IEEE Power & Energy Society (bottom centre).
- Voice and beep alerts:

| Time left | Sound | Voice |
|---|---|---|
| 15 min | 1 big beep | "15 minutes remaining" |
| 10 min | 1 big beep | "10 minutes remaining" |
| 5 min | 3 big beeps | "5 minutes remaining" |
| 0 | 2 big beeps, then 5 fast beeps | "Time's up. Best of luck!" |

- Full-screen "Best of Luck!" ending with confetti and animated light rays.
- Presets of 5, 10, 15, 20, 30, 45 and 60 minutes, plus a custom time of 1 to 180 minutes.
- Editable event title, start/pause, reset, test sound, mute and full screen.
- The progress ring turns amber in the last 5 minutes and red in the last minute.
- Responsive on phones, tablets and projectors.

## Keyboard shortcuts

| Key | Action |
|---|---|
| Space | Start / pause (or close the ending screen) |
| R | Reset |
| F | Full screen |
| Esc | Close the ending screen |

## Usage

1. Open `index.html` in a browser, or visit the hosted page.
2. Choose a preset or enter a custom number of minutes.
3. Click **Test sound** once to allow audio and check the speakers.
4. Click **Start**.

Notes:

- Browsers only allow sound after a click, so press Start or Test sound before the event.
- If the timer is set below 15 minutes, the alerts that have already passed are skipped.
- The spoken voice depends on the device's built-in voices.
- Google Fonts load when online. Offline, the page falls back to system fonts.

## Hosting on GitHub Pages

1. Push `index.html` to the `main` branch of your repository.
2. Open **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then **Save**.
4. After a minute or two the timer is live at `https://<your-username>.github.io/<repository-name>/`.

## Customising

All styles and scripts are inside `index.html`.

- **Alert times:** change the values `900`, `600` and `300` (seconds) in the script.
- **Voice text:** edit the `say(...)` lines in the `notify` and `finish` functions.
- **Colours:** edit the variables at the top of the `<style>` block (`--green`, `--blue`, `--amber`, `--red`).
- **Credit line:** edit the `credit` block near the end of the page.

## Credits

Created by Miadul Nizzan, Vice Chair, IEEE GUB Student Branch.

Logos belong to Green University of Bangladesh, IEEE GUB Student Branch, IEEE Computer Society and IEEE Power & Energy Society.
