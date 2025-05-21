# JUPIFY Installation Guide

This guide provides detailed instructions to set up JUPIFY locally for development or deployment.

## Prerequisites

Before installing JUPIFY, ensure you have the following:

- **Node.js**: Version 18 or higher
- **PostgreSQL**: Version 14 or higher
- **Git**: For cloning the repository

## Step-by-Step Installation

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/jupify.git
cd jupify
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Database Setup

#### 3.1 Create a PostgreSQL Database

```sql
CREATE DATABASE jupify;
```

#### 3.2 Configure Environment Variables

Create a `.env` file in the root directory with the following variables:

```
DATABASE_URL=postgresql://username:password@localhost:5432/jupify
```

Replace `username` and `password` with your PostgreSQL credentials.

#### 3.3 Initialize the Database Schema

```bash
npm run db:push
```

This command uses Drizzle ORM to push the schema defined in `shared/schema.ts` to your database.

### 4. Start the Development Server

```bash
npm run dev
```

This will start both the frontend development server with Vite and the backend Express server.

### 5. Access the Application

Open your browser and navigate to:

```
http://localhost:3000
```

## Production Deployment

### Building for Production

```bash
npm run build
```

This creates optimized production builds for both frontend and backend in the `dist` directory.

### Running in Production

```bash
npm run start
```

## Troubleshooting

### Common Issues

1. **Database Connection Problems**
   - Verify your PostgreSQL service is running
   - Check that your DATABASE_URL environment variable is correct
   - Ensure your database user has appropriate permissions

2. **Port Conflicts**
   - If port 3000 is already in use, you can modify the port in `server/index.ts`

3. **Wallet Connection Issues**
   - For wallet integration testing, use a browser with wallet extensions installed
   - Ensure you're on a supported network (Solana mainnet or testnet)

## Further Support

If you encounter any issues or have questions, please:
- Open an issue on GitHub
- Refer to the documentation in the `docs` directory
- Join the JUPIFY community Discord for real-time support