
# 💰 Personal Finance Tracker

A modern, responsive personal finance tracker built with Next.js, featuring a beautiful dark theme with gradient backgrounds. Track your income, expenses, and manage your financial categories with ease.

![Personal Finance Tracker](https://i.pinimg.com/736x/f0/96/11/f096111bddda9d3d1ad31b7a07fa1c81.jpg)

## ✨ Features

- 🌙 **Modern Dark Theme** - Beautiful dark design with purple gradient backgrounds
- 💸 **Transaction Management** - Add, view, edit, and delete income/expense transactions
- 📊 **Dashboard Analytics** - Visual overview of your financial status
- 🏷️ **Category Management** - Organize transactions with custom categories
- 📋 **PDF Reports** - Generate and download detailed financial reports
- 📱 **Responsive Design** - Works perfectly on desktop and mobile
- ⚡ **Real-time Updates** - Instant UI updates with optimistic rendering
- 🔍 **Search & Filter** - Find transactions quickly with built-in search

## 🛠️ Tech Stack

- **Framework**: Next.js 14 with App Router
- **Database**: PostgreSQL with Prisma ORM
- **Styling**: Tailwind CSS with custom dark theme
- **UI Components**: Radix UI primitives with shadcn/ui
- **TypeScript**: Full type safety
- **Charts**: Chart.js for data visualization
- **Deployment**: Vercel recommended

## 🚀 Getting Started

### Prerequisites

- Node.js 18+ 
- yarn or npm
- PostgreSQL database

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/personal-finance-tracker.git
   cd personal-finance-tracker
   ```

2. **Install dependencies**
   ```bash
   cd app
   yarn install
   # or
   npm install
   ```

3. **Set up environment variables**
   ```bash
   cp .env.example .env
   ```
   
   Update `.env` with your database URL:
   ```env
   DATABASE_URL="postgresql://username:password@localhost:5432/finance_tracker"
   ```

4. **Set up the database**
   ```bash
   npx prisma migrate dev
   npx prisma generate
   npx prisma db seed
   ```

5. **Run the development server**
   ```bash
   yarn dev
   # or
   npm run dev
   ```

6. **Open your browser**
   Navigate to [http://localhost:3000](http://localhost:3000)

## 🎨 Design System

The app features a cohesive dark theme with:

- **Primary Colors**: Green accent (#22c55e) for interactive elements
- **Background**: Dynamic gradient from slate-900 through purple-900
- **Cards**: Semi-transparent dark cards with subtle borders
- **Typography**: High contrast white text for optimal readability
- **Glass Effects**: Backdrop blur for modern aesthetics

## 📁 Project Structure

```
personal-finance-tracker/
├── app/
│   ├── app/                    # Next.js App Router
│   │   ├── api/               # API routes
│   │   ├── globals.css        # Global styles & theme
│   │   ├── layout.tsx         # Root layout
│   │   └── page.tsx          # Home page
│   ├── components/            # React components
│   │   ├── ui/               # Reusable UI components
│   │   ├── dashboard-view.tsx # Dashboard interface
│   │   ├── transactions-view.tsx # Transaction management
│   │   └── categories-view.tsx # Category management
│   ├── lib/                   # Utilities and database
│   ├── prisma/               # Database schema
│   └── hooks/                # Custom React hooks
└── README.md
```

## 🐳 Running with VS Code

1. **Open in VS Code**
   ```bash
   code personal-finance-tracker
   ```

2. **Install recommended extensions**
   - TypeScript and JavaScript Language Features
   - Tailwind CSS IntelliSense
   - Prisma
   - ES7+ React/Redux/React-Native snippets

3. **Open integrated terminal** (`Ctrl+\``) and navigate to app directory:
   ```bash
   cd app
   yarn dev
   ```

4. **Use VS Code Live Server** or open [http://localhost:3000](http://localhost:3000)

## 📊 Database Schema

The app uses the following main entities:

- **Transactions**: Income/expense records with amounts, descriptions, dates
- **Categories**: Organize transactions (Food, Transport, Salary, etc.)
- **User Settings**: Application preferences and configuration

## 🌐 Deployment

### Vercel (Recommended)

1. **Push to GitHub** (see instructions below)

2. **Connect to Vercel**
   - Go to [vercel.com](https://vercel.com)
   - Import your GitHub repository
   - Add environment variables in Vercel dashboard

3. **Live Demo**: [https://your-app.vercel.app](https://your-app.vercel.app)

### Other Platforms

The app can be deployed on:
- Netlify
- Railway
- Heroku
- DigitalOcean App Platform

## 📚 API Endpoints

- `GET/POST /api/transactions` - Transaction CRUD operations
- `GET/POST /api/categories` - Category management
- `GET /api/summary` - Financial summary data
- `GET /api/report/pdf` - Generate PDF reports

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Built with [Next.js](https://nextjs.org/)
- UI components from [shadcn/ui](https://ui.shadcn.com/)
- Icons from [Lucide React](https://lucide.dev/)
- Styled with [Tailwind CSS](https://tailwindcss.com/)

## 📞 Support

If you have any questions or need help, please open an issue on GitHub.

---

**⭐ Star this repository if you found it helpful!**
