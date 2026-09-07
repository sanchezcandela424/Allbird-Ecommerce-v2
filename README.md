# Allbird E-Commerce Platform 🛍️

**Core Features**
- 🛍️ Product catalog with search, filtering & categories
- 🛒 Shopping cart with persistent storage
- 📧 Newsletter subscription with validation
- 🎨 Custom 404 page with demo messaging
- 👤 User authentication with NextAuth.js
- 💳 Stripe payment integration (configured)
- 📊 Admin dashboard for product & order management

**Tech Stack**
- **Frontend:** Next.js 15.5.6 | React 18 | TypeScript 5.9  | Tailwind CSS | shadcn/ui
- **Backend:** Server Components | Server Actions | API Routes
- **Database:** PostgreSQL 15 | Prisma 5.22 ORM
- **Testing:** Jest | React Testing Library | Cypress

### Prerequisites
- Node.js 20+ 
- PostgreSQL 15+
- npm or yarn

### Installation

```bash
# Clone the repository
git clone https://github.com/SatvikPraveen/Nextjs-Ecommerce.git
cd Nextjs-Ecommerce

# Install dependencies
npm install

# Set up environment variables
cp .env.example .env.local
# Edit .env.local with your database URL and API keys

# Set up database
npx prisma db push
npm run db:seed

# Start development server
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) to see the app.

### Essential Environment Variables

```env
# Database (Required)
DATABASE_URL="postgresql://user:password@localhost:5432/ecommerce"

# NextAuth (Required)
NEXTAUTH_SECRET="your-secret-here"
NEXTAUTH_URL="http://localhost:3000"

# Stripe (Optional - for payments)
STRIPE_PUBLISHABLE_KEY="pk_test_..."
STRIPE_SECRET_KEY="sk_test_..."
```
