# AeroGuardian AI - Drone Detection & Emergency Response System

🚁 **Intelligent AI Assistant for Drone Emergencies & Safety**

[![Live Demo](https://img.shields.io/badge/Live%20Demo-🚀-blue?style=for-the-badge)](https://sanyamsuyal.github.io/aeroguardian-ai/)
[![GitHub Stars](https://img.shields.io/github/stars/sanyamsuyal/aeroguardian-ai?style=for-the-badge)](https://github.com/sanyamsuyal/aeroguardian-ai/stargazers)
[![MIT License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)

## 🎯 What is AeroGuardian AI?

AeroGuardian AI is an intelligent emergency response system that provides:

- **Expert drone safety guidance** and threat assessment
- **Real-time first aid instructions** for drone-related injuries
- **Indian emergency services integration** with instant contact access
- **Professional incident reporting** and safety protocols
- **24/7 AI-powered assistance** for drone emergencies

## 📦 Requirements

- **Node.js 18+** (JavaScript runtime)
- **npm 8+** (Package manager)
- **Git** (for cloning the repository)
- **Together AI API Key** (for chatbot functionality)

## 🚀 Complete Step-by-Step Setup Guide

### 📋 Prerequisites (Install First)

#### 1. Install Node.js and npm

- **Download**: Visit [nodejs.org](https://nodejs.org/)
- **Choose**: Download **LTS version** (Long Term Support)
- **Install**: Run the installer, follow setup wizard
- **Verify installation**:

```bash
node --version
# Should show v18.0.0 or higher

npm --version  
# Should show v8.0.0 or higher
```

#### 2. Install Git

- **Download**: Visit [git-scm.com](https://git-scm.com/)
- **Install**: Follow installation wizard for your OS
- **Verify installation**:

```bash
git --version
# Should show git version 2.x.x
```

#### 3. Get Together AI API Key

- **Visit**: [together.ai](https://together.ai)
- **Sign up**: Create free account
- **Login**: Access your dashboard
- **Navigate**: Go to API Keys section
- **Generate**: Create new API key
- **Copy**: Save the key securely (you'll need it later)

### 🔧 Fork and Setup Process

#### Step 1: Fork the Repository

1. Go to [github.com/sanyamsuyal/aeroguardian-ai](https://github.com/sanyamsuyal/aeroguardian-ai)
2. Click **"Fork"** button (top-right corner)
3. Select your GitHub account as destination
4. Wait for GitHub to create your copy

#### Step 2: Clone Your Fork

```bash
# Replace YOUR_USERNAME with your GitHub username
git clone https://github.com/YOUR_USERNAME/aeroguardian-ai.git

# Navigate into the project
cd aeroguardian-ai
```

#### Step 3: Navigate to Frontend

```bash
cd frontend
```

#### Step 4: Install Dependencies

```bash
# Install all required packages (takes 2-5 minutes)
npm install
```

**What gets installed:**

- React 18.2.0 - Main framework
- Tailwind CSS - Styling framework  
- Chart.js - Data visualization
- Framer Motion - Animations
- Axios - API requests
- Socket.io - Real-time features
- Plus 15+ other essential packages

#### Step 5: Setup Environment Variables

```bash
# Copy template file
cp .env.example .env

# Windows users:
copy .env.example .env
```

**Edit .env file:**

1. Open `.env` in any text editor
2. Replace `your_together_ai_api_key_here` with your actual API key
3. Save the file

**Final .env should look like:**

```env
REACT_APP_TOGETHER_API_KEY=your_actual_api_key_here
REACT_APP_TOGETHER_API_URL=https://api.together.xyz/v1/chat/completions
```

#### Step 6: Start Development Server

```bash
npm start
```

**What happens:**

- Development server starts
- Browser opens automatically to `http://localhost:3000`
- App loads with hot-reload enabled
- Changes auto-refresh the browser

### ✅ Verify Everything Works

1. **Terminal**: Should show "Compiled successfully!"
2. **Browser**: App loads at localhost:3000
3. **Chat**: Type a message and press enter
4. **AI Response**: Should receive AI replies
5. **Emergency Mode**: Click emergency button to test

### 🐛 Common Issues & Solutions

#### "npm command not found"

**Problem**: Node.js not installed properly

**Solution**: 

```bash
# Reinstall Node.js from nodejs.org
# Restart terminal after installation
node --version
```

#### "npm install fails"

**Problem**: Package installation errors

**Solution**:

```bash
# Clear cache and retry
npm cache clean --force
rm -rf node_modules package-lock.json
npm install
```

#### "API not working"

**Problem**: Environment variables not loaded

**Solution**:

```bash
# Check .env file exists
ls -la .env

# Verify content (without sharing key)
cat .env

# Restart server
npm start
```

#### "Port 3000 already in use"

**Problem**: Another app using same port

**Solution**:

```bash
# Kill process on port 3000
npx kill-port 3000

# Or use different port
PORT=3001 npm start
```

### 📁 Understanding Project Structure

```
aeroguardian-ai/
├── frontend/
│   ├── src/
│   │   ├── App.js          # Main chatbot logic
│   │   ├── App.css         # All styling & animations
│   │   └── index.js        # React entry point
│   ├── .env                # Your API keys (SECRET)
│   ├── .env.example        # Template for setup
│   └── package.json        # Dependencies list
├── .github/workflows/      # Auto-deployment
├── README.md              # This guide
└── LICENSE                # MIT license
```

### 🎯 Key Files Explained

- **App.js**: Contains AI integration, emergency features, chat logic
- **App.css**: Visual styling, animations, responsive design
- **.env**: Your secret API keys (NEVER commit to git)
- **package.json**: Lists all dependencies and scripts

### 🛠️ Making Your Own Changes

#### To modify chatbot behavior:

1. Edit `frontend/src/App.js`
2. Find system prompts (around line 100-150)
3. Modify emergency actions or responses
4. Save - changes appear automatically

#### To change appearance:

1. Edit `frontend/src/App.css`
2. Modify colors, animations, layouts
3. Save - styling updates immediately

#### To add new packages:

```bash
# Install new package
npm install package-name

# Import in App.js
import NewFeature from 'package-name';

# Use in your code
```

### 🚀 Deploy Your Version

#### GitHub Pages (Free):

1. Push changes to your GitHub fork
2. Go to repository Settings > Pages
3. Enable GitHub Pages
4. Add API key in repository Secrets
5. Auto-deploys on every push to main

#### Vercel (Recommended):

1. Connect GitHub repo to Vercel
2. Import project
3. Add environment variables in dashboard
4. Deploy with one click

### 📞 Getting Help

**If stuck:**

1. Check browser console (F12 key)
2. Read terminal error messages
3. Search error messages online
4. Create issue in repository
5. Check troubleshooting section above

### 💡 Beginner Tips

- **Save often** - Changes auto-reload
- **Use browser console** - F12 shows errors
- **Read error messages** - They usually explain the problem
- **Test frequently** - Don't write lots of code without testing
- **Start small** - Make one change at a time

### 🎉 Success!

After completing these steps you'll have:

- ✅ Working AI chatbot with emergency features
- ✅ Professional UI with animations
- ✅ Full development environment
- ✅ Ability to customize and deploy
- ✅ All drone safety and first aid capabilities

**You're ready to build amazing things! 🚀**

## 🔧 Advanced Development

### Local Development

```bash
# Start development server
npm start

# Build for production
npm run build

# Test the build locally
npm run serve
```

### Environment Variables

Create a `.env` file in the frontend directory:

```env
REACT_APP_TOGETHER_API_KEY=your_api_key_here
REACT_APP_TOGETHER_API_URL=https://api.together.xyz/v1/chat/completions
```

### Deployment

The app is configured for GitHub Pages deployment. Push to `main` branch to auto-deploy.

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Built with React and Together AI
- Emergency services data for India
- Drone safety protocols and guidelines
- First aid medical procedures

---

**Made with ❤️ for drone safety and emergency response**
