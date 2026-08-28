# StakeShack

Trustless renting platform. Replaces the third-party guarantor with on-chain crypto staking, so a renter posts a stake instead of paying a middleman to vouch for them. Adds referral rewards and AI-powered listing recommendations.

**2nd place, $1,500, OnionDAO Solana Hackathon.** Built solo in 48 hours.

**Stack:** Next.js · TypeScript · Supabase / PostgreSQL · Solana · Anchor · Rust · Gill

## How it works

- A renter stakes SOL against a listing rather than routing a deposit through a guarantor.
- Escrow release and slashing conditions live in the Anchor program, so neither party has to trust the other.
- Listing data and user profiles sit in Supabase, with recommendations ranked over that data.

## Setup

```bash
bun install
bun dev
```

Open http://localhost:3000. Database schema is in `database-setup.sql`. The on-chain program is in `escrow`.
