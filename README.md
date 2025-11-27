# Micro-Commitment Creative Passions

*Automatically synced with your [v0.app](https://v0.app) deployments*

[![Deployed on Vercel](https://img.shields.io/badge/Deployed%20on-Vercel-black?style=for-the-badge&logo=vercel)](https://vercel.com/chandanasreev11-9167s-projects/v0-micro-commitment-creative-passions)
[![Built with v0](https://img.shields.io/badge/Built%20with-v0.app-black?style=for-the-badge)](https://v0.app/chat/uX7VsMvs369)

## Overview

This repository will stay in sync with your deployed chats on [v0.app](https://v0.app).
Any changes you make to your deployed app will be automatically pushed to this repository from [v0.app](https://v0.app).

## Features

**Daily Micro-Challenges**
- AI-generated creative challenges personalized to your artistic style
- Categories: Sketching, Music Composition, Creative Writing
- New challenge every day to build consistent creative habits

**Personalized AI Feedback**
- Instant feedback on your creative submissions
- AI scoring system (0-100) based on creativity, execution, and style alignment
- Detailed constructive feedback to help you improve

**Streak Tracking & Habit Building**
- Visual streak counter showing your creative consistency
- Motivation levels based on psychology-driven engagement models
- Achievements unlocked at milestones (7-day Warrior, 30-day Master, etc.)
- Longest streak tracking for personal records

**Creative History**
- View all your past submissions and feedback
- Track your creative journey over time
- Review AI scores and improvement areas

**Personalization System**
- Define your unique artistic style (e.g., abstract, minimalist, surreal)
- AI engine personalizes challenges based on your style profile
- Recommendations adapt as you submit more work

## Deployment

Your project is live at:

**[https://vercel.com/chandanasreev11-9167s-projects/v0-micro-commitment-creative-passions](https://vercel.com/chandanasreev11-9167s-projects/v0-micro-commitment-creative-passions)**

## Build your app

Continue building your app on:

**[https://v0.app/chat/uX7VsMvs369](https://v0.app/chat/uX7VsMvs369)**

## Getting Started

### Installation

1. **Clone and Install**
   \`\`\`bash
   git clone <repository-url>
   cd Art-Streak
   npm install
   \`\`\`

2. **Run Development Server**
   \`\`\`bash
   npm run dev
   \`\`\`

3. **Open in Browser**
   Visit `http://localhost:3000` to start using the app

### First Time Setup

1. Create your account with your name and email
2. Enter your artistic style (e.g., abstract, experimental, minimalist, surreal)
3. Get your first daily challenge
4. Submit your creative work
5. Receive AI feedback and start your streak

## Tech Stack

- **Frontend**: Next.js 16 with React 19
- **Styling**: Tailwind CSS v4 with custom theme
- **State Management**: localStorage for data persistence
- **UI Components**: Custom React components with Tailwind styling
- **AI Integration**: Mock AI feedback system (ready for real LLM integration)
- **Deployment**: Vercel

## Project Structure

\`\`\`
├── app/
│   ├── layout.tsx           # Root layout with theme setup
│   ├── page.tsx             # Main app page with dashboard
│   └── globals.css          # Global styles and theme variables
├── components/
│   ├── auth-form.tsx        # User authentication and setup
│   ├── challenge-card.tsx   # Daily challenge display
│   ├── submission-modal.tsx # Challenge submission interface
│   ├── streak-widget.tsx    # Streak tracking and stats display
│   ├── history-view.tsx     # Past submissions and feedback
│   └── ui/                  # Reusable UI components
├── lib/
│   ├── types.ts             # TypeScript interfaces
│   ├── storage.ts           # localStorage utilities
│   └── utils.ts             # Helper functions
└── public/                  # Static assets
\`\`\`

## How It Works

### Authentication Flow
- Users sign up with name, email, and artistic style preference
- Data stored in localStorage for persistence
- Session maintained across browser refreshes

### Challenge Generation
- AI engine generates unique daily challenges
- Challenges personalized based on user's artistic style
- New challenge appears each calendar day

### Submission & Feedback
- Users submit creative work with descriptions
- AI provides feedback with score (0-100)
- Feedback factors: creativity, execution, style alignment

### Streak System
- Streak increases with daily submissions
- Resets after missing a day
- Longest streak tracked separately
- Motivation levels unlock achievements

## Data Structure

### User Profile
\`\`\`typescript
{
  id: string;
  name: string;
  email: string;
  artisticStyle: string;
  currentStreak: number;
  longestStreak: number;
  totalSubmissions: number;
  createdAt: number;
}
\`\`\`

### Challenge
\`\`\`typescript
{
  id: string;
  date: string;
  category: 'sketch' | 'music' | 'writing';
  prompt: string;
  difficultyLevel: 'beginner' | 'intermediate' | 'advanced';
}
\`\`\`

### Submission
\`\`\`typescript
{
  id: string;
  challengeId: string;
  userDescription: string;
  aiFeedback: string;
  aiScore: number;
  submittedAt: number;
  category: string;
}
\`\`\`

## Customization

### Change Theme Colors
Edit `app/globals.css` to modify the CSS custom properties:
- `--primary`: Main brand color (default: purple)
- `--secondary`: Accent color (default: orange)
- `--background`: Background color
- `--foreground`: Text color

### Modify Challenge Types
Update `components/challenge-card.tsx` to add new challenge categories or customize the prompt generation logic.

### Adjust Streak Milestones
Edit `components/streak-widget.tsx` to change achievement thresholds and titles.

## Future Enhancements

- Real AI API integration (OpenAI, Anthropic, etc.)
- Database persistence (Supabase, Neon)
- User authentication with OAuth
- Social features (share achievements, follow creators)
- Advanced analytics and insights
- Mobile app version
- Collaborative challenges
- Leaderboards and community engagement

## Contributing

This project is built on v0.app. To contribute:
1. Visit the project on [v0.app](https://v0.app/chat/uX7VsMvs369)
2. Make your changes in the chat interface
3. Deploy from v0.app
4. Changes automatically sync to this repository

## License

MIT License - feel free to use this project for personal or commercial purposes.

## Support

For issues or questions:
- Visit [v0.app](https://v0.app) to view the live development
- Check the GitHub repository for issues
- Review the code structure in this repository

---

**Built with v0.app** - AI-powered design and development tool
