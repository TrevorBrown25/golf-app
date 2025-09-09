# Golf App

A fantasy golf app featuring weekly head-to-head drafts with 4 starters per lineup. Money equals points - final placing payout (USD) becomes points for that event. Missed cut = $0 = 0 points.

## MVP Scope

- [ ] User authentication & profiles
- [ ] Weekly H2H draft system
- [ ] 4-starter lineup management
- [ ] Scoring based on tournament payouts
- [ ] Matchup scheduling & results
- [ ] Basic leaderboards

## Phase Map

- **P0** - Repo skeleton & tooling setup
- **P1** - Next.js scaffold with health route
- **P2** - Database schema & Prisma setup
- **P3** - Authentication with NextAuth
- **P4** - Core data models & tRPC APIs
- **P5** - Draft system & lineup management
- **P6** - Scoring engine & tournament data
- **P7** - Matchup system & scheduling
- **P8** - UI/UX with shadcn/ui components
- **P9** - Production deployment & monitoring

## Confirmed Decisions

- **Data Source**: Stub adapter first, real tournament data later
- **Scoring**: Final placing payout (USD) = points for that event; missed cut = $0 = 0 pts
- **Roster/Lineups**: 4 starters, weekly reset, lock at first tee time, H2H vs opponent; golfers return to pool after each event
- **Branding**: Golf App

## Tech Stack

- **Frontend**: Next.js App Router + TypeScript
- **API**: tRPC
- **Database**: Prisma + PostgreSQL
- **Auth**: NextAuth
- **Styling**: Tailwind CSS + shadcn/ui
- **Package Manager**: pnpm
- **Development**: Docker Desktop
- **Deploy**: Vercel + Supabase/Neon

## Getting Started (Git Bash on Windows)

### Prerequisites

1. **Install nvm-windows**:
   ```bash
   # Download and install from: https://github.com/coreybutler/nvm-windows/releases
   # Or use winget: winget install CoreyButler.NVMforWindows
   ```

2. **Install pnpm**:
   ```bash
   npm install -g pnpm
   ```

3. **Install Docker Desktop**:
   ```bash
   # Download from: https://www.docker.com/products/docker-desktop/
   # Or use winget: winget install Docker.DockerDesktop
   ```

### Setup

1. **Install and use Node LTS**:
   ```bash
   nvm install 20.16.0
   nvm use 20.16.0
   ```

2. **Verify tool versions**:
   ```bash
   node --version    # Should show v20.16.0
   pnpm --version    # Should show latest pnpm
   docker --version  # Should show Docker version
   ```

3. **Test Docker**:
   ```bash
   docker run hello-world
   ```

## Next Steps

Ready for **P1 scaffold** - Next.js project setup with health route and basic tooling configuration.