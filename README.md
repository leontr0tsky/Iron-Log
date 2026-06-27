# IronLog — Strength Training Tracker

A premium strength training tracker built for powerlifters, bodybuilders, and serious gym-goers. Fast, data-driven workout logging focused on progressive overload.

**[Live Demo →](https://yourusername.github.io/ironlog/IronLog.html)**

![IronLog Dashboard](https://via.placeholder.com/800x450/111111/e8ff47?text=IronLog)

---

## Features

**Workout Logging**
- Log exercises, sets, reps, weight, and RPE/RIR
- Real-time session timer and volume tracking
- Previous workout comparison inline
- Warmup set tracking separate from working sets
- Session notes and rating

**Analytics & Progress**
- Strength progress charts per exercise (Est. 1RM over time)
- Weekly volume bar charts (4, 8, 12 week views)
- Muscle group volume breakdown
- Training streak tracker
- Weekly activity calendar

**Personal Records**
- Auto-detects new PRs when you save a workout
- Big 3 total (Squat + Bench + Deadlift)
- Per-exercise history of top sets
- Estimated 1RM using Epley formula

**Calculators**
- 1RM Calculator — Epley, Brzycki, Lombardi, O'Conner formulas
- Full percentage table (60–100%) with rep zone guidance
- Plate Calculator with visual bar diagram
- Warm-up Set Generator

**Exercise Library**
- 20 exercises with full technique instructions
- Filter by muscle group and equipment
- Coaching tips for each movement
- Compound and isolation categorized

**Body Tracker**
- Weight and body fat trend charts
- Full measurement log (chest, waist, hips, biceps, thighs)
- Delta tracking vs previous measurement

**Rest Timer**
- Floating SVG ring timer
- Presets: 1m, 1:30, 2m, 3m, 4m, 5m
- ±15 second adjustments
- Vibration alert on completion (mobile)

---

## Tech Stack

- **React 18** + **TypeScript**
- **Tailwind CSS** — utility-first styling
- **Framer Motion** — animations and micro-interactions
- **Recharts** — analytics charts
- **LocalStorage** — data persistence, no backend needed

---

## Running Locally

```bash
git clone https://github.com/yourusername/ironlog.git
cd ironlog
npm install
npm start
```

Or just open `IronLog.html` directly in your browser — no build step needed.

---

## Keyboard Shortcuts

| Key | Action |
|-----|--------|
| `N` | New workout |
| `T` | Toggle rest timer |
| `Esc` | Close sidebar / modal |

---

## Project Structure

```
src/
├── App.tsx                  # Root component, navigation, state
├── types/index.ts           # TypeScript interfaces
├── data/
│   ├── exercises.ts         # Exercise library (20 movements)
│   └── seedData.ts          # Demo data
├── utils/index.ts           # 1RM formulas, plate calc, helpers
└── components/
    ├── Dashboard.tsx        # Overview, stats, charts
    ├── WorkoutLogger.tsx    # Active workout logging
    ├── ExerciseLibrary.tsx  # Browse and filter exercises
    ├── Calculators.tsx      # 1RM, plates, warmup
    ├── PersonalRecords.tsx  # PR tracker
    ├── Progress.tsx         # Strength and volume charts
    ├── WorkoutHistory.tsx   # Past sessions
    ├── BodyTracker.tsx      # Measurements
    ├── RestTimer.tsx        # Floating rest timer
    └── ui.tsx               # Reusable UI components
```

---

## Design

- Dark mode by default — matte black (`#111111`) with charcoal surfaces
- Accent color: electric yellow-green (`#e8ff47`)
- Monospace font (JetBrains Mono) for all numbers and stats
- Mobile-first, fully responsive
- No glassmorphism, no gradients, no bloat

---

## License

MIT — free to use, modify, and distribute.
