# cooldown-manager
A lightweight, offline-capable task cooldown tracker — create cards for repetitive actions, set hh:mm:ss timers, track daily usage, and get notified when you're ready to go again. Pure HTML/CSS/JS, no dependencies.

Project Link: https://elfilaliamin.github.io/cooldown-manager/

the used Prompt:

Create a single-file **HTML web app** (all HTML, CSS, and JavaScript in one `.html` file) that helps me track cooldown timers for repetitive tasks.

## Main Purpose

The app should let me create task cards for actions such as:

- Uploading to Zazzle
- Posting designs
- Rendering images
- Any custom action

Each task/card must have:

1. Task name
2. Cooldown duration (example: 1 hour, 30 minutes, etc.)
3. Optional image URL
4. Start button
5. Live countdown timer
6. Daily usage counter (how many times I clicked Start today)

---

## Features Required

### 1. Add New Task Cards

Create a form where I can:

- Enter task name
- Enter cooldown duration in minutes
- Enter optional image URL
- Click “Add Card”

When added, generate a visually clean card.

---

### 2. Card Layout

Each card should display:

- Image (if provided)
- Task title
- Cooldown duration
- Current status:
    - “Ready”
    - or remaining countdown time
- “Start” button
- “Reset” button
- Counter:
    - “Started today: X times”

---

### 3. Countdown Logic

When I click the “Start” button:

- The countdown begins immediately
- The button becomes disabled during cooldown
- The timer updates live every second
- When the cooldown finishes:
    - The card changes to “Ready”
    - The button becomes active again
    - Play a small notification sound
    - Show a browser notification if permissions are allowed

---

### 4. Daily Counter

For each card:

- Count how many times I pressed “Start” today
- Automatically reset the counter at midnight
- Store the data persistently

---

### 5. Persistent Storage (IMPORTANT)

Use `localStorage` to store ALL app data, including:

- Created cards
- Cooldown timers
- Active countdown end times
- Daily usage counters
- Sound preferences
- User settings

Requirements:

- Data must persist after page refresh or browser restart
- Active countdowns must continue correctly after reopening the HTML file
- Save updates automatically whenever data changes
- Load all saved data automatically when the app starts

---

### 6. UI / Design

Requirements:

- Modern responsive design
- Dark mode interface
- Smooth animations
- Clean dashboard layout
- Cards in a responsive grid
- Use pure HTML/CSS/JavaScript only
- No frameworks
- No external backend

---

### 7. Extra Features

Add:

- Delete card button
- Edit card button
- Search/filter cards
- Sort by:
    - Ready first
    - Cooldown remaining
    - Most used today
- Progress bar for cooldown
- Sound toggle ON/OFF

---

### 8. Technical Requirements

- Everything must be inside ONE `.html` file
- Use semantic HTML
- Write clean, well-structured code
- Include comments for important sections
- Avoid external dependencies when possible
- The app must work offline after opening the HTML file

---

### 9. Example Use Case

Example card:

- Task: “Upload to Zazzle”
- Cooldown: 60 minutes
- Image: thumbnail URL
- After clicking Start:
    - countdown starts from 60:00
    - daily counter increases
    - timer persists even if page reloads

---

### 10. Deliverable

Output only the complete final `.html` code file.

### Modifications:

1. Improve Cooldown Duration input to include (hh:mm:ss)
2. Better theme like used in react webapps with calm colors such (Pintrest, Facebook, instagram...)
3. Better card layout (when I add Image URL (direct link) it's not appearing in the task card
