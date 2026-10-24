# typing-speed-game

A quick, clean typing speed test. Type the words, watch your WPM and accuracy
update live, race the clock, and try to beat your best score. Pick 15, 30 or 60
seconds. It runs entirely in your browser.

**Live:** https://siddique-12300983.github.io/typing-speed-game/

## How to play

Click the card and start typing the words shown. The timer starts on your first
keypress. Each character turns green when it is right and red when it is wrong,
and a caret shows where you are. When the time runs out you get your score, and
your best WPM is saved on your device so you have something to beat.

## Features

- Live WPM, accuracy and countdown
- 15, 30 and 60 second modes
- Per-character feedback as you type, with a blinking caret
- Real accuracy: mistakes count even if you backspace and fix them
- Best score saved locally (nothing leaves your browser)
- Restart any time, and a fresh set of words each round
- Dark theme, works on desktop and mobile

## How WPM is measured

WPM uses the standard "word = 5 characters" convention: it counts the correctly
typed characters, divides by five to get words, and divides by the minutes
elapsed. Accuracy is counted at the keystroke level (correct keystrokes out of
total keystrokes), so fixing a typo does not erase the mistake, which keeps the
number honest.

## Running it locally

One HTML file, no build step, no libraries.

```bash
python -m http.server 8000
# then open http://localhost:8000
```

## Tech

Plain HTML, CSS and JavaScript. Best score uses `localStorage`. No network
requests, no dependencies.

## License

MIT. See [LICENSE](LICENSE).
