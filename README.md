# PaintStuff


Why I Built This

I recently started learning to draw and paint. I quickly found a wall in my progress, not because of a lack of content available on the internet, but because of an overwhelming pool of resources, a lack of structure, and no personalized feedback.

I believe one of the most important potentials of AI is to act as a personalized teacher that can meet anybody at their knowledge level and teach them almost anything. I wanted to build a system that uses computer vision to look at a user's drawings, diagnose what's technically wrong, and explain how to improve with actionable insights.



 Project Structure

```
ai-art-tutor/
├── app/                      # Expo Router screens
│   ├── _layout.tsx          # Root layout
│   └── (tabs)/              # Tab navigation
│       ├── _layout.tsx      # Tab bar configuration
│       ├── index.tsx        # Home (progress ring, stats)
│       ├── practice.tsx      # Practice (mode selection, upload, AI feedback)
│       └── history.tsx      # History (learning journal)
├── components/               # Reusable UI components
│   ├── GlassCard.tsx        # Glassmorphism card
│   ├── ProgressRing.tsx     # SVG progress indicator
│   ├── CountdownTimer.tsx   # Practice timer
│   └── SessionCompleteModal.tsx  # Manual time entry
├── context/                  # Global state management
│   └── AppContext.tsx       # Skill level, progress, history
├── services/                 # API integrations
│   ├── api.ts               # Unsplash, Groq AI, AsyncStorage
│   └── types.ts             # TypeScript interfaces
├── constants/                # App constants
│   └── theme.ts             # Colors, skill levels, prompts
├── .env                     # API keys (not committed)
├── .env.example             # Template for .env
└── package.json
```


