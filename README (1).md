# JUPIFY - Gamified Learning Hub for Jupiter's DeFi Ecosystem

JUPIFY is an engaging, gamified learning platform focused on educating users about Jupiter's DeFi ecosystem through interactive quests, rewards, and community features.

![JUPIFY Logo](client/public/jupify-logo.png)

## Features

- **Interactive Quest System**: Complete educational quests to learn about Jupiter's DeFi products
- **Knowledge Nebula**: Visual skill tree showing different learning paths through the Jupiter ecosystem
- **Reward System**: Earn XP and JUP tokens for completing quests and achievements
- **Quest Momentum**: Streak visualization with cosmic animations for consistent learning
- **Leaderboards**: Compete with other learners in the community
- **Wallet Integration**: Connect with Phantom, Solflare, or JUP Mobile wallets
- **Engaging UI**: Space-themed, responsive design with dark mode

## Tech Stack

- **Frontend**: React, TypeScript, Tailwind CSS, ShadCN UI, Framer Motion
- **Backend**: Node.js with Express
- **Database**: PostgreSQL with Drizzle ORM
- **Authentication**: Wallet-based authentication
- **State Management**: React Context API, TanStack Query

## Getting Started

### Prerequisites

- Node.js (v18+)
- PostgreSQL

### Installation

1. Clone the repository
```
git clone https://github.com/yourusername/jupify.git
cd jupify
```

2. Install dependencies
```
npm install
```

3. Set up environment variables
```
DATABASE_URL=postgresql://username:password@localhost:5432/jupify
```

4. Initialize the database
```
npm run db:push
```

5. Start the development server
```
npm run dev
```

## Project Structure

```
.
├── client/                 # Frontend code
│   ├── public/             # Static assets
│   └── src/
│       ├── components/     # UI components
│       ├── contexts/       # React contexts for state management
│       ├── hooks/          # Custom hooks
│       ├── lib/            # Utility functions and types
│       └── pages/          # Page components
├── server/                 # Backend code
│   ├── mockdata/           # Test/demo data
│   ├── index.ts            # Main server entry point
│   ├── routes.ts           # API routes
│   └── storage.ts          # Data storage interface
└── shared/                 # Shared code between frontend and backend
    └── schema.ts           # Database schema and types
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Jupiter Protocol for inspiration and ecosystem
- The JUPIFY community of learners and contributors