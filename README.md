# Phas-VoiceTimer

This is a Voice activated timer I made to use for phasmophobia



========================================

&#x20;VOICE ACTIVATED TIMER

========================================



A hands-free, voice-controlled timer with a small always-on-top toast

notification and spoken alerts at key time milestones. Say a command,

and a timer starts, counts down out loud, and lets you know when it's

done -- no need to touch your keyboard or mouse.



Handy for anything with timed phases you need to track without looking

away from what you're doing (e.g. games with cooldown/hunt-style

mechanics, real-world timed rituals or routines, or any other repeated

countdown you'd rather not babysit manually).





\----------------------------------------

&#x20;FEATURES

\----------------------------------------



\- Voice-activated start/stop for four different timer types

\- Spoken countdown milestones (not just a silent visual timer)

\- Small floating "toast" notification window, always on top, semi-transparent

\- Choice of natural-sounding online voices (via Microsoft Edge's TTS) or

&#x20; any offline system voice installed on your PC

\- Adjustable voice speaking speed

\- Six built-in themes (Default White, Dark Mode, Pastel Green/Pink/Blue/Red)

\- Remembers your microphone, voice, speed, and theme between launches

\- Auto-installs its own Python dependencies on first run -- no manual

&#x20; "pip install" required

\- Custom app icon and taskbar icon





\----------------------------------------

&#x20;VOICE COMMANDS

\----------------------------------------



&#x20; "timer start" / "start timer" / "smudge start" / "start smudge" /

&#x20; "incense start" / "start incense"

&#x20;     -> Starts a 3-minute timer.

&#x20;        Spoken alerts at 60s, 90s, 120s, and 180s (done).



&#x20; "cooldown start" / "cool down start"

&#x20;     -> Starts a short cooldown timer.

&#x20;        Spoken alerts at 20s and 25s (done).



&#x20; "paranormal sound start" / "paranormal sounds start" /

&#x20; "sound start" / "sounds start"

&#x20;     -> Starts a 2-minute sound timer.

&#x20;        Spoken alerts at 80s and 120s (done).



&#x20; "hunt start" / "start hunt"

&#x20;     -> Starts a 2-minute timer.

&#x20;        Spoken alerts at 15, 20, 30, 40, 50, 60s, then every 20s until done.



&#x20; "timer stop" / "stop timer"

&#x20;     -> Immediately stops whichever timer is currently active,

&#x20;        with a short beep confirmation.



(This same list is also available in-app any time via the "?" button.)





\----------------------------------------

&#x20;REQUIREMENTS

\----------------------------------------



\- Python 3.8 or newer (Windows, macOS, or Linux)

\- A working microphone

\- An internet connection for:

&#x20;   \* Google's free speech-recognition API (used to understand your

&#x20;     voice commands)

&#x20;   \* Microsoft Edge's online voices, if you pick one of those for alerts

&#x20;     (offline system voices work fully without internet)



You do NOT need to manually install any Python packages -- the app

checks for everything it needs (SpeechRecognition, PyAudio, gTTS,

pyttsx3, edge-tts) the first time it runs, and installs anything

missing automatically via pip. If pip itself isn't available, it will

first try to bootstrap it using Python's built-in "ensurepip" module

before giving up and telling you exactly what to install manually.





\----------------------------------------

&#x20;HOW TO RUN

\----------------------------------------



1\. Install Python 3.8+ or the most latest one (preferable) if you don't already have it:

&#x20;  https://www.python.org/downloads/

&#x20;  (On Windows, make sure to tick "Add python.exe to PATH" during setup.)



2\. Download the newest/latest release of the app from this repository.

   • Latest Release > [**Download**](https://github.com/perpy08/Phas-VoiceTimer/releases/tag/PhasVoiceTimer0.0.1) <

   -Extract Anywhere you'd prefer



3\. Run it:

&#x20;  double-click it (Timer.exe), depending on your system's file associations



4\. The first run will show a small "Installing Required Dependencies"

&#x20;  popup while it sets itself up. This only happens once.



5\. Once the main window appears:

&#x20;  - Select your microphone from the dropdown

&#x20;  - Pick an alert voice (Preview button lets you hear it first)

&#x20;  - Click "Start Listen"

&#x20;  - Say any of the voice commands above








\----------------------------------------

&#x20;TROUBLESHOOTING

\----------------------------------------



\- "It doesn't hear anything I say"

&#x20;   Double check the correct microphone is selected in the dropdown,

&#x20;   and that your OS isn't muting/blocking mic access for the app.



\- "Voice commands stopped working mid-session"

&#x20;   This usually means the recognition service hit a network hiccup.

&#x20;   The status label and button will reset themselves back to

&#x20;   "Start Listen" automatically if this happens -- just click it again.



\- "pip install failed" / "pip not found"

&#x20;   Make sure you have an internet connection, and that Python was

&#x20;   installed with pip included (the default python.org installer

&#x20;   includes it; some minimal/embeddable Python builds do not).





\----------------------------------------

&#x20;CREDITS

\----------------------------------------



Program made by Perpy08.



Built with:

&#x20; - SpeechRecognition (https://pypi.org/project/SpeechRecognition/)

&#x20; - PyAudio

&#x20; - gTTS / edge-tts (text-to-speech)

&#x20; - pyttsx3 (offline text-to-speech)

&#x20; - Tkinter (bundled with Python)

