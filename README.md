# Mock Interview Drill

**AppADay 170** | Educational | Claude API

Paste any job description and Claude drafts 8 to 10 likely interview questions split into behavioral and technical sets. Each card has its own practice timer with a suggested answer length, autosaving notes, and a practiced toggle that feeds a progress counter. Export your prep as Markdown.

## How to use it

**Add your key.** Tap the gear in the header and paste your Anthropic API key. You can show or hide it while typing and clear it at any time. Get a key at [console.anthropic.com](https://console.anthropic.com/).

**Paste the posting.** Drop the full job description into the input card (at least 80 characters, up to 12,000) and tap Generate Questions. Claude returns behavioral questions to answer with the STAR method and technical questions tied to the tools and skills in the posting, each with a note on what the interviewer is listening for.

**Practice out loud.** Every card has its own timer set to a suggested answer length between one and five minutes. Starting one timer pauses any other, the clock turns coral when you run over, and phones vibrate once at the limit. Jot talking points in the notes box, which saves as you type, and tap Mark practiced when you are happy with an answer. The progress strip and section counts update as you go.

**Export.** Copy Markdown puts your full prep sheet on the clipboard, and Download .md saves it as mock-interview-drill-YYYY-MM-DD.md with each question, its suggested length, practiced status, and your notes. Reset clears the posting, questions, notes, and progress but keeps your API key. Generating again asks before replacing your current set.

## Privacy

Your API key, the posting, and your notes are stored only in this browser's localStorage. The posting is sent directly from your browser to api.anthropic.com and nowhere else.

## Model

The model is not hardcoded. The app reads the sonnet tier from the AppADay central [config.json](https://augustineiacopelli.github.io/appaday/config.json) and falls back to claude-sonnet-5-5 if the file cannot be reached. Thinking is turned off with a per model fallback so the full token budget goes to the questions.

## Links

Live app: https://augustineiacopelli.github.io/appaday-170-mock-interview-drill/

Portfolio: https://augustineiacopelli.github.io/appaday/
