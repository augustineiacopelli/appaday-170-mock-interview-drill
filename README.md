# Mock Interview Drill

**AppADay 170** | Educational | Claude API

Paste any job description and Claude drafts 8 to 10 likely interview questions split into behavioral and technical sets. Each card has its own practice timer with a suggested answer length, autosaving notes, and a practiced toggle that feeds a progress counter. Export your prep as Markdown.

## How to use it

**Connect your key.** The first time you generate, a sheet slides up offering to restore your keys from your AppADay key file or to enter a key. You can also do this any time from the gear in the header, which shows whether this app uses its own key or your default key (last four characters only) and lets you enter a key, restore from or back up to your key file, or forget a key. Keys are checked with Anthropic before they are saved. Get a key at [console.anthropic.com](https://console.anthropic.com/).

**Paste the posting.** Drop the full job description into the input card (at least 80 characters, up to 12,000) and tap Generate Questions. Claude returns behavioral questions to answer with the STAR method and technical questions tied to the tools and skills in the posting, each with a note on what the interviewer is listening for.

**Practice out loud.** Every card has its own timer set to a suggested answer length between one and five minutes. Starting one timer pauses any other, the clock turns coral when you run over, and phones vibrate once at the limit. Jot talking points in the notes box, which saves as you type, and tap Mark practiced when you are happy with an answer. The progress strip and section counts update as you go.

**Export.** Copy Markdown puts your full prep sheet on the clipboard, and Download .md saves it as mock-interview-drill-YYYY-MM-DD.md with each question, its suggested length, practiced status, and your notes. Reset clears the posting, questions, notes, and progress but keeps your API key. Generating again asks before replacing your current set.

## API key

Key handling comes from the shared AppADay key ring, [keys.js](https://augustineiacopelli.github.io/appaday/keys.js), described in KEYS.md in the portal repo. The key lives under appaday.key.170 with a fallback to your default key, and can be backed up to a passphrase encrypted file, appaday-keys.json, that restores every AppADay app's key at once. A key saved by an earlier version of this app is carried over automatically.

## Privacy

Your API key, the posting, and your notes are stored only in this browser's localStorage. The key and the posting are sent directly from your browser to api.anthropic.com and nowhere else. The key file's passphrase is never stored.

## Model

The model is not hardcoded. The app asks the portal's shared models.js for the sonnet tier, which follows the AppADay central [config.json](https://augustineiacopelli.github.io/appaday/config.json). Thinking is turned off with a per model fallback so the full token budget goes to the questions.

## Links

Live app: https://augustineiacopelli.github.io/appaday-170-mock-interview-drill/

Portfolio: https://augustineiacopelli.github.io/appaday/
