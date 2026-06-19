# 🎓 Axiom - Interactive AI Learning Platform

> The future of personalized education is here. **Learn smarter, not harder.**

![Axiom Status](https://img.shields.io/badge/Status-Building-blue?style=flat-square)
![Tech Stack](https://img.shields.io/badge/Tech-Next.js%20%7C%20Express%20%7C%20OpenAI-purple?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)

## 🌟 What is Axiom?

Axiom is an **AI-powered interactive learning platform** that revolutionizes how students learn:

✨ **Upload & Explain** - Send confusing topics, get instant AI explanations  
🎤 **Voice Learning** - Speak naturally, learn through conversation  
🧠 **Smart Practice** - Practice with adaptive questions without judgment  
📝 **Note Enhancement** - Get AI suggestions to improve your study materials  
📊 **Real-time Testing** - Take oral and written tests with instant feedback  

## 🎯 The Problem We Solve

Students struggle with:
- ❌ Finding relevant educational content on YouTube
- ❌ Getting stuck at specific parts without immediate clarification
- ❌ Fear of asking questions in class
- ❌ No practice partner for oral preparation
- ❌ Passive note-taking without guidance
- ❌ Isolated learning experience

**Axiom solves ALL of these problems** ✅

## 🚀 Key Features

### 📸 Image-Based Explanations
- Upload any concept image you're confused about
- AI analyzes and explains in simple, step-by-step terms
- Get alternative explanations and deeper insights
- Ask follow-up questions without judgment

### 🎤 Voice Interface
- Speak naturally and get spoken responses
- Conversational learning without fear of judgment
- Oral tests that adapt to your learning pace
- Learn while commuting or doing chores

### 🧠 Interactive Practice Mode
- AI asks questions like a real teacher
- Get immediate feedback on your answers
- Stop anytime to discuss difficult parts
- Progress tracking and personalized recommendations
- Never gets frustrated - only encourages learning

### 📚 Smart Notes System
- Upload your notes for AI analysis
- Get organization and clarity suggestions
- Receive alternative explanations
- Auto-generate study guides from notes
- Improve note-taking skills over time

### 📊 Comprehensive Testing
- Written tests with detailed explanations
- Oral assessments with adaptive difficulty
- Real-time performance analytics
- Personalized learning path recommendations
- Test history and improvement tracking

## 🛠️ Tech Stack

**Frontend:**
- Next.js 14 (React with App Router)
- React Three Fiber (3D animations)
- Tailwind CSS (Responsive design)
- Framer Motion (Smooth interactions)
- Web Speech API (Voice I/O)

**Backend:**
- Node.js + Express.js
- PostgreSQL (User data, progress, tests)
- Redis (Real-time features, caching)
- OpenAI API (Explanations, tests, voice)
- ElevenLabs (Voice synthesis)
- AWS S3 (File storage)

**DevOps:**
- Docker & Docker Compose
- GitHub Actions (CI/CD)
- Vercel (Frontend deployment)
- Railway/Render (Backend deployment)

## 📁 Project Structure

```
axiom-learning-platform/
├── frontend/                    # Next.js 14 Application
│   ├── app/
│   │   ├── layout.tsx          # Root layout
│   │   ├── page.tsx            # Landing page
│   │   ├── (auth)/
│   │   │   ├── login/
│   │   │   └── signup/
│   │   └── (dashboard)/
│   │       ├── dashboard/
│   │       ├── explain/
│   │       ├── practice/
│   │       ├── test/
│   │       ├── notes/
│   │       └── progress/
│   ├── components/
│   │   ├── branding/           # Axiom logo & theme
│   │   ├── navigation/         # Navbar, sidebar
│   │   ├── sections/           # Landing page sections
│   │   ├── layout/             # Layout components
│   │   ├── ui/                 # Reusable UI elements
│   │   └── interactive/        # 3D & animations
│   ├── hooks/                  # Custom React hooks
│   ├── lib/                    # Utilities & API client
│   ├── types/                  # TypeScript interfaces
│   ├── styles/                 # Global styles
│   └── public/                 # Static assets
│
├── backend/                    # Express.js API Server
│   ├── src/
│   │   ├── index.ts           # Entry point
│   │   ├── config/            # Configuration
│   │   ├── routes/
│   │   │   ├── auth.ts        # Authentication
│   │   │   ├── explanations.ts # Image explanations
│   │   │   ├── practice.ts    # Practice questions
│   │   │   ├── tests.ts       # Test management
│   │   │   ├── notes.ts       # Note analysis
│   │   │   └── users.ts       # User profiles
│   │   ├── controllers/       # Business logic
│   │   ├── models/            # Database models
│   │   ├── middleware/        # Auth, validation
│   │   ├── services/          # AI integrations
│   │   └── utils/             # Helper functions
│   ├── migrations/            # Database migrations
│   ├── seeds/                 # Initial data
│   ├── Dockerfile
│   └── tsconfig.json
│
├── database/
│   ├── schema.sql             # Database schema
│   └── seeds.sql              # Initial data
│
├── docs/
│   ├── ARCHITECTURE.md        # System design
│   ├── DATABASE.md            # Schema reference
│   ├── API.md                 # API documentation
│   ├── SETUP.md               # Installation guide
│   └── DESIGN.md              # Design system
│
├── .github/workflows/
│   ├── ci.yml                 # CI/CD pipeline
│   └── deploy.yml             # Deployment workflow
│
├── docker-compose.yml         # Local development setup
├── package.json               # Root package config
├── .gitignore
├── .env.example
├── CONTRIBUTING.md            # Contribution guidelines
├── LICENSE                    # MIT License
└── README.md
```

## 🚀 Quick Start

### Prerequisites
- **Node.js** 18+ (LTS recommended)
- **Docker & Docker Compose** (optional)
- **Git** for version control
- **API Keys** (optional): OpenAI, ElevenLabs

### Installation

```bash
# 1. Clone repository
git clone https://github.com/kishorenath011-droid/axiom-learning-platform.git
cd axiom-learning-platform

# 2. Install root dependencies
npm install

# 3. Setup frontend
cd frontend
npm install
cp .env.example .env.local
# Edit .env.local with your API keys (optional)

# 4. Setup backend (new terminal)
cd backend
npm install
cp .env.example .env
# Edit .env with your API keys (optional for development)

# 5. Start database services (optional, uses Docker)
docker-compose up -d

# 6. Run database migrations (if using Docker)
cd backend
npm run db:migrate

# 7. Start frontend development server
cd frontend
npm run dev
# Opens http://localhost:3000

# 8. Start backend development server (new terminal)
cd backend
npm run dev
# Server runs on http://localhost:3001
```

### Using Docker Compose

```bash
# Start all services
docker-compose up

# Frontend: http://localhost:3000
# Backend: http://localhost:3001
# PostgreSQL: localhost:5432
# Redis: localhost:6379
```

## 🎨 Design System

### Axiom Brand Identity

**Logo**: Stylized 'A' with light rays (knowledge radiating) + lightbulb (ideas)

**Color Palette:**

| Element | Color | Hex | Usage |
|---------|-------|-----|-------|
| Primary Gradient | Blue-Purple | #5967ff → #3d2aff | Headers, CTAs, main UI |
| Accent Gradient | Orange | #ff8800 → #ffaa1a | Highlights, decorations |
| Success | Emerald | #10b981 | Correct answers, success states |
| Warning | Amber | #f59e0b | Warnings, tips, notices |
| Error | Red | #ef4444 | Errors, wrong answers |
| Info | Blue | #3b82f6 | Information, tips |

**Typography:**
- **Headings**: Serif fonts (elegant, educational)
- **Body**: System sans-serif (clean, readable)
- **Code**: Monospace (technical content)

### Component Library

- Buttons (Primary, Secondary, Icon, Gradient)
- Cards (Standard, Interactive, 3D)
- Forms (Input, Textarea, Select, File Upload)
- Navigation (Navbar, Sidebar, Breadcrumbs)
- Animations (Fade, Slide, Scale, Float)
- 3D Elements (Rotating shapes, parallax effects)

## 📚 Documentation

- [Architecture Guide](./docs/ARCHITECTURE.md) - System design, data flow, scalability
- [Database Schema](./docs/DATABASE.md) - Data models and relationships
- [API Reference](./docs/API.md) - Complete endpoint documentation
- [Setup Guide](./docs/SETUP.md) - Detailed installation & configuration
- [Design System](./docs/DESIGN.md) - UI components, colors, typography
- [Contributing](./CONTRIBUTING.md) - How to contribute to the project

## 🔄 Data Flow Examples

### Image Explanation Flow
```
User uploads image
    ↓
Backend validates image (size, format)
    ↓
Stores in S3 or local storage
    ↓
Calls OpenAI Vision API
    ↓
AI generates explanation
    ↓
Caches in Redis (24 hours)
    ↓
Sends to Frontend with streaming
    ↓
Frontend displays with typing animation
    ↓
User can request voice playback via ElevenLabs
```

### Practice Mode Flow
```
User selects topic & difficulty
    ↓
Backend checks Redis cache for questions
    ↓
If not cached, calls OpenAI to generate
    ↓
Caches generated questions (7 days)
    ↓
Sends questions to Frontend
    ↓
User answers question
    ↓
Backend sends to OpenAI for evaluation
    ↓
AI provides feedback & explanation
    ↓
Updates user progress in DB
    ↓
Adjusts difficulty based on performance
    ↓
Offers next question or review
```

### Voice Learning Flow
```
User speaks
    ↓
Web Speech API transcribes audio (browser)
    ↓
Sends text to Backend
    ↓
Backend calls OpenAI for response
    ↓
Gets AI-generated text response
    ↓
Calls ElevenLabs API for voice synthesis
    ↓
Returns audio file to Frontend
    ↓
Frontend plays audio through speaker
    ↓
User can repeat, slow down, or ask follow-up
```

## 🔐 Security Features

✅ **JWT Authentication** - Secure token-based auth with refresh tokens  
✅ **HTTPS/TLS** - All communications encrypted  
✅ **Rate Limiting** - Prevent abuse on API endpoints  
✅ **Input Validation** - Sanitize all user inputs  
✅ **CORS Configuration** - Restrict cross-origin requests  
✅ **Environment Variables** - Keep secrets secure  
✅ **Database Encryption** - Encrypt sensitive user data  
✅ **File Upload Validation** - Virus scanning, size limits  

## 📊 Performance Optimizations

- **Frontend**: Next.js image optimization, code splitting, lazy loading
- **Backend**: Connection pooling, query optimization, caching strategies
- **Database**: Proper indexing, query optimization, data partitioning
- **CDN**: CloudFlare for static assets and API acceleration
- **Caching**: Redis for session, frequently accessed data, generated content

## 🧪 Testing

```bash
# Run all tests
npm test

# Run specific test suite
npm test -- auth
npm test -- explanations

# Coverage report
npm test -- --coverage

# E2E tests (coming soon)
npm run test:e2e
```

## 🚀 Deployment

### Frontend (Vercel)
```bash
npm run build
vercel deploy
```

### Backend (Railway/Render)
```bash
docker build -t axiom-backend ./backend
# Push to container registry
# Deploy via Railway, Render, or Heroku
```

### Database
- **PostgreSQL**: AWS RDS, Railway, or Heroku Postgres
- **Redis**: AWS ElastiCache, Railway Redis, or Upstash

## 🤝 Contributing

We love contributions! Here's how:

1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/amazing-feature`)
3. **Commit** your changes (`git commit -m 'feat: add amazing feature'`)
4. **Push** to the branch (`git push origin feature/amazing-feature`)
5. **Open** a Pull Request

See [CONTRIBUTING.md](./CONTRIBUTING.md) for detailed guidelines.

## 📝 Commit Message Format

```
<type>(<scope>): <subject>

<body>

<footer>
```

**Types**: `feat`, `fix`, `docs`, `style`, `refactor`, `test`, `chore`

**Example**:
```
feat(explanations): implement image-based AI explanations

- Integrate OpenAI vision API for image analysis
- Add image upload handler with validation
- Implement Redis caching for explanations
- Add streaming response to frontend

Closes #42
```

## 🐛 Issue Reporting

Found a bug? [Create an issue](https://github.com/kishorenath011-droid/axiom-learning-platform/issues) with:
- 📝 Clear description of the problem
- 🔄 Steps to reproduce
- ✅ Expected vs actual behavior
- 📸 Screenshots (if applicable)
- 💻 Environment details (OS, browser, Node version)

## 📄 License

MIT License © 2024 Axiom Learning Platform

See [LICENSE](./LICENSE) file for details.

---

## 🎯 Roadmap

### Phase 1: MVP (Current)
- [x] Project setup & architecture
- [ ] Authentication (signup/login)
- [ ] Image-based explanations
- [ ] Voice interface basics
- [ ] Practice mode

### Phase 2: Enhanced Learning
- [ ] Test system with analytics
- [ ] Notes analysis & suggestions
- [ ] Progress tracking dashboard
- [ ] Personalized recommendations
- [ ] Community features

### Phase 3: Advanced Features
- [ ] Mobile app (React Native)
- [ ] Offline mode
- [ ] Advanced analytics
- [ ] AI-generated content
- [ ] Group study sessions

### Phase 4: Scale
- [ ] Enterprise features
- [ ] Integration with schools
- [ ] API for third parties
- [ ] Advanced AI models
- [ ] Multi-language support

## 👥 Team

Built with ❤️ by students, for students.

We're passionate about making quality education accessible to everyone.

---

**Ready to learn smarter? Start with Axiom today!** 🚀

[🌐 Website](https://axiom.dev) | [📧 Contact](mailto:hello@axiom.dev) | [💬 Discussions](https://github.com/kishorenath011-droid/axiom-learning-platform/discussions)
