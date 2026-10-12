# Study-Garden

The complete application is `dist/index.html`. Copy it as `index.html` to the root of a GitHub Pages publishing source. No build, backend, dependencies, accounts, or API keys are required.

## Assignment specifications

Purpose: a student focus timer, task organizer, and illustrated reward garden.

- Task titles: 1–80 trimmed characters; optional subject up to 30 characters. Add, edit, delete, complete, reopen, and filter tasks. The task in a current session is locked.
- Focus: 15/25/50-minute presets or a whole-number duration from 1 to 120 minutes. Start, pause, resume, and confirmed reset. Default 25 minutes. One active timer per page.
- Three plants: Daisy, Sunflower, Cactus. Growth stages: seed 0–24%, sprout 25–49%, young 50–74%, mature 75–100%.
- Exactly one earned plant per completed focus session; no reward for reset, break, or demo. Task completion stays manual.
- Optional 5-minute break; starts only on request. Pausable and skippable.
- Unsaved 10-second demo for quickly reviewing the main interaction.
- Garden grid with clickable session details; history filters for today and all time.
- Completed study minutes and sessions today; total plants and total focus time; daily goal from 1 to 720 minutes (default 60).
- Completion date uses the device local timezone. Goal bar caps at 100%, actual minutes remain visible.
- Versioned browser localStorage saves tasks, settings, timer, and completed session snapshots. Timestamp recovery reconciles elapsed time after refreshing or returning.
- Light/dark themes, optional completion sound, keyboard focus, labeled controls, responsive layouts, reduced-motion support, visible completion messages.
- Confirmed data reset; storage and input error feedback. No transmission of study data. No synchronization between browsers or devices. Intended for one active tab.
- All CSS, JavaScript, and original SVG graphics are embedded in a single HTML file. No ML is used inside the app. AI assisted specification, design, implementation, and verification.

## Actual development refinements and checks

After the feature specification, the app was implemented with special handling for timer timestamps, completed-session IDs, immutable historical task labels, and whitespace-only task input. An inappropriate registered-trademark mark was removed from the header before delivery. Built-in project notes were updated with actual validation rather than claiming browser testing.

JavaScript syntax passed. Seventeen scripted functional assertions passed in a simulated DOM: empty task validation, task creation, invalid duration, task-linked session, pause, paused time, single completion reward, correct minutes/manual task completion, demo exclusion, break exclusion, timer restoration, deduplication after restoration, cancel reset, confirmed reset, goal saving, theme/history persistence, and HTML escaping.

Limit: browser rendering, keyboard traversal, mobile layout, audio, and a real interface screenshot have not been verified in a browser in this session. No screenshot is fabricated. Run the 10-second demo to review animation and use a 1-minute session to verify a real reward. The demo intentionally adds no plant.


- Open the public link while signed out to verify accessibility.
- Take a screenshot of the actual interface, preferably after a completed 1-minute session.
- Paste the public link, screenshot, specifications, and actual revision summary into the assignment text input.
- Title: [School abbreviation] [Student ID] [Department abbreviation] Angelina Panyananda Study Garden.
- Do not claim checks or publication that have not happened.
