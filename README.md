# MENTORx37

> AI-Powered Career Assistant for smarter job search, resume optimization, mock interviews, and industry insights.

![Next.js](https://img.shields.io/badge/Next.js-16-black?style=flat-square&logo=next.js)
![React](https://img.shields.io/badge/React-19-61DAFB?style=flat-square&logo=react)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-3.4-38B2AC?style=flat-square&logo=tailwind-css)
![Prisma](https://img.shields.io/badge/Prisma-6.2-2D3748?style=flat-square&logo=prisma)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)

## Features

- **AI Resume Builder** - Create professional resumes with AI-powered suggestions and improvements
- **AI Cover Letter Generator** - Generate tailored cover letters for any job position
- **Mock Interview Prep** - Practice interviews with AI-generated questions and get instant feedback
- **Industry Insights Dashboard** - Real-time salary data, market trends, and skill recommendations
- **Secure Authentication** - Powered by Clerk for seamless sign-in experience

## Tech Stack

| Category | Technologies |
|----------|-------------|
| Frontend | Next.js 16, React 19, Tailwind CSS, Framer Motion, GSAP |
| UI Components | Shadcn UI, Radix UI, Lucide Icons |
| Backend | Next.js API Routes, Server Actions |
| Database | PostgreSQL (NeonDB), Prisma ORM |
| Authentication | Clerk |
| AI | Google Gemini API |
| Deployment | Vercel |

## Quick Start

### Prerequisites

- Node.js 18+
- PostgreSQL database (NeonDB recommended)
- Clerk account
- Google Gemini API key

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/ashutosh936/MENTORx37.git
cd MENTORx37
```

2. **Install dependencies**
```bash
npm install
```

3. **Set up environment variables**

Create a `.env` file in the root directory:
```env
# Database
DATABASE_URL="postgresql://..."

# Clerk Authentication
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=pk_...
CLERK_SECRET_KEY=sk_...
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/onboarding
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/onboarding

# Gemini AI
GEMINI_API_KEY=your_gemini_api_key
```

4. **Set up the database**
```bash
npx prisma generate
npx prisma db push
```

5. **Run the development server**
```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

## Project Structure

```
MENTORx37/
├── app/                    # Next.js App Router
│   ├── (auth)/            # Authentication pages
│   ├── (main)/            # Main app pages
│   │   ├── dashboard/     # User dashboard
│   │   ├── resume/        # Resume builder
│   │   ├── interview/     # Interview prep
│   │   ├── ai-cover-letter/ # Cover letter generator
│   │   └── onboarding/    # User onboarding
│   ├── api/               # API routes
│   └── lib/               # App utilities
├── actions/               # Server actions
├── components/            # React components
│   └── ui/               # Shadcn UI components
├── data/                  # Static data
├── hooks/                 # Custom React hooks
├── lib/                   # Utilities & configs
└── prisma/               # Database schema
```

## Screenshots

| Dashboard | Resume Builder |
|-----------|---------------|
| Industry insights & analytics | AI-powered resume creation |

| Interview Prep | Cover Letter |
|----------------|--------------|
| Mock interviews with AI | Generate tailored letters |

## Deployment

### Deploy to Vercel

1. Push your code to GitHub
2. Connect your repository to [Vercel](https://vercel.com)
3. Add environment variables in Vercel dashboard
4. Deploy

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new)

## Author

**Ashutosh Sharma**

- GitHub: [@ashutosh936](https://github.com/ashutosh936)

## License

This project is licensed under the MIT License.

---

If you found this project helpful, please give it a star!
