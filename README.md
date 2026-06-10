# QuickPay Admin

**Real-time payment processing admin dashboard.**

A production-grade administrative interface for managing payment transactions, users, and analytics. Built with React, TypeScript, and Supabase for real-time data synchronization.

## Features

- Real-time transaction monitoring dashboard
- User management with role-based access control
- Payment analytics and reporting (Recharts)
- Responsive design with Tailwind CSS
- Supabase backend with lazy authentication initialization
- Serverless-ready (Netlify Functions)

## Tech Stack

- **Frontend:** React 18, TypeScript, Vite, Tailwind CSS, Recharts
- **Backend:** Supabase (PostgreSQL + Auth)
- **Deployment:** Netlify (functions + hosting)
- **Icons:** Lucide React

## Getting Started

```bash
# Clone the repo
git clone https://github.com/SucceedHQ/QUICKPAY-ADMIN.git
cd QUICKPAY-ADMIN

# Install dependencies
npm install

# Set up environment
cp .env.example .env.local
# Add your Supabase credentials to .env.local

# Start development server
npm run dev
```

### Environment Variables

| Variable | Description |
|----------|-------------|
| `VITE_SUPABASE_URL` | Supabase project URL |
| `VITE_SUPABASE_ANON_KEY` | Supabase anonymous API key |

## Available Scripts

| Command | Description |
|---------|-------------|
| `npm run dev` | Start Vite dev server |
| `npm run build` | TypeScript check + production build |
| `npm run lint` | Run ESLint across the project |
| `npm run preview` | Preview production build locally |

## Project Structure

```
src/
├── components/    # Reusable UI components
├── pages/         # Route page components
├── lib/           # Supabase client & utilities
├── hooks/         # Custom React hooks
└── types/         # TypeScript type definitions
```

## Deployment

The project is configured for deployment on Netlify:

```bash
# Build for production
npm run build

# The netlify.toml handles routing and function configuration
```

## License

MIT
