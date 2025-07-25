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

## 🔧 Advanced Developmentsistance System

[![GitHub Pages](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-blue?style=for-the-badge)](https://sanyamsuyal.github.io/aeroguardian-ai)
[![React](https://img.shields.io/badge/React-18.0+-61DAFB?style=for-the-badge&logo=react)](https://reactjs.org)
[![Together AI](https://img.shields.io/badge/Together%20AI-Mistral%207B-orange?style=for-the-badge)](https://together.ai)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)

🛡️ **Advanced AI-powered drone emergency assistance system with real-time threat detection and comprehensive first aid guidance.**

Created by **Sanyam Suyal**

## 🌟 Live Demo

**🚀 [Try AeroGuardian AI Live](https://sanyamsuyal.github.io/aeroguardian-ai)**

*Experience the full power of AI-driven drone emergency assistance*

## 🚀 Features

- **Smart Drone Intelligence** - Expert-level drone type identification and threat assessment
- **Emergency First Aid** - Comprehensive medical guidance for drone-related injuries
- **Indian Emergency Integration** - Complete helpline directory with specialized services
- **Real-time AI Assistance** - Advanced chatbot with typewriter effects and professional formatting
- **Emergency Mode** - Immediate crisis response with panic button functionality
- **Professional UI** - Vibrant animations, responsive design, and accessibility features

## 🛠️ Technology Stack

- **Frontend**: React 18, JavaScript ES6+, CSS3 with animations
- **AI Integration**: Together AI (Mistral 7B model)
- **Styling**: Custom CSS with advanced animations and effects
- **APIs**: RESTful integration with environment variables

## 📋 Prerequisites

Before running this project, make sure you have the following installed:

- **Node.js** (version 16.0 or higher)
- **npm** (version 8.0 or higher) or **yarn**
- **Git** (for cloning the repository)
- **Together AI API Key** (for chatbot functionality)

## � Quick Start (GitHub)

### For Contributors:

1. **Fork this repository** on GitHub
2. **Clone your fork**:
   ```bash
   git clone https://github.com/YOUR_USERNAME/aeroguardian-ai.git
   cd aeroguardian-ai
   ```
3. **Setup environment**:
   ```bash
   cd frontend
   cp .env.example .env
   # Edit .env with your Together AI API key
   npm install
   npm start
   ```

### For Users:

- **🌟 [Use Live Version](https://sanyamsuyal.github.io/aeroguardian-ai)** - No installation needed!
- **⬇️ Download Latest Release** - Get stable version from [Releases](https://github.com/sanyamsuyal/aeroguardian-ai/releases)

## 🔧 Local Development Setup

### Step 1: Clone the Repository

```bash
git clone https://github.com/sanyamsuyal/aeroguardian-ai.git
cd aeroguardian-ai
```

### Step 2: Navigate to Frontend Directory
```bash
cd frontend
```

### Step 3: Install Dependencies
```bash
npm install
```

**Required Dependencies:**
- `react` (^18.0.0)
- `react-dom` (^18.0.0)
- `react-scripts` (^5.0.0)

### Step 4: Set Up Environment Variables

Create a `.env` file in the `frontend` directory:

```bash
# Create .env file
touch .env
```

Add the following environment variables to `.env`:

```env
REACT_APP_TOGETHER_API_KEY=your_together_ai_api_key_here
REACT_APP_TOGETHER_API_URL=https://api.together.xyz/v1/chat/completions
```

**🔑 Getting Together AI API Key:**
1. Visit [together.ai](https://together.ai)
2. Sign up for an account
3. Navigate to API section
4. Generate your API key
5. Replace `your_together_ai_api_key_here` with your actual API key

### Step 5: Start the Development Server
```bash
npm start
```

The application will open in your browser at `http://localhost:3000`

## 🏗️ Project Structure

```
aeroguardian-ai/
├── frontend/
│   ├── public/
│   │   ├── index.html
│   │   └── favicon.ico
│   ├── src/
│   │   ├── App.js              # Main React component
│   │   ├── App.css             # Styling and animations
│   │   └── index.js            # React entry point
│   ├── .env                    # Environment variables (not in git)
│   ├── .env.example            # Environment template
│   ├── package.json            # Dependencies and scripts
│   └── package-lock.json       # Dependency lock file
├── .github/
│   └── workflows/
│       └── deploy.yml          # GitHub Actions workflow
├── .gitignore                  # Git ignore file
└── README.md                   # This file
```

## 🎮 Usage Guide

### Normal Mode
- **Safety Tips**: Get comprehensive drone safety information
- **Threat Assessment**: Real-time system status and threat evaluation
- **Chat Interface**: Ask questions about drones, safety, or first aid

### Emergency Mode
- **Take Cover**: Immediate tactical positioning guidance
- **First Aid**: Medical assistance for drone-related injuries
- **Emergency Services**: Quick access to Indian emergency contacts
- **Panic Button**: Instant emergency alert system

### Key Features
- **Typewriter Animation**: Smooth word-by-word text display
- **Professional Formatting**: Bold text, numbered lists, and proper line breaks
- **Indian Emergency Numbers**: 112, 100, 108, 101, 1070, 1091, etc.
- **Drone Expertise**: Consumer, racing, professional, and military drone identification

## 🚨 Emergency Contacts (India)

| Service | Number | Description |
|---------|--------|-------------|
| **National Emergency** | 112 | Police, Fire, Medical |
| **Police** | 100 | Law enforcement |
| **Ambulance** | 108 | Medical emergency |
| **Fire Brigade** | 101 | Fire and rescue |
| **Disaster Management** | 1070 | Natural disasters |
| **Women's Helpline** | 1091 | Women's safety |
| **Anti-Terror Squad** | 1090 | Terror threats |
| **Railway Emergency** | 139 | Train emergencies |
| **Tourist Helpline** | 1363 | Tourist assistance |

## 🐛 Troubleshooting

### Common Issues & Solutions

**1. API Key Not Working**
```bash
# Check if .env file exists and has correct format
cat .env
# Restart development server
npm start
```

**2. Dependencies Not Installing**
```bash
# Clear npm cache
npm cache clean --force
# Delete node_modules and reinstall
rm -rf node_modules package-lock.json
npm install
```

**3. Build Errors**
```bash
# Check Node.js version
node --version
# Should be 16.0 or higher

# Check npm version
npm --version
# Should be 8.0 or higher
```

**4. Environment Variables Not Loading**
- Ensure `.env` file is in the `frontend` directory
- Restart development server after adding environment variables
- Check that variables start with `REACT_APP_`

## 🚀 Deployment

### Deploy to GitHub Pages (Free)

1. **Fork this repository** on GitHub
2. **Enable GitHub Pages** in repository settings
3. **Add secrets** in repository settings > Secrets and variables > Actions:
   - `REACT_APP_TOGETHER_API_KEY`: Your Together AI API key
   - `REACT_APP_TOGETHER_API_URL`: `https://api.together.xyz/v1/chat/completions`

4. **Push to main branch** - GitHub Actions will automatically deploy

### Deploy to Vercel (Recommended)

1. **Connect GitHub repository** to Vercel
2. **Import project** from GitHub
3. **Add environment variables** in Vercel dashboard:
   - `REACT_APP_TOGETHER_API_KEY`: Your Together AI API key
   - `REACT_APP_TOGETHER_API_URL`: `https://api.together.xyz/v1/chat/completions`
4. **Deploy automatically** on every push

### Deploy to Netlify

1. **Connect GitHub repository** to Netlify
2. **Set build settings**:
   - Build command: `cd frontend && npm run build`
   - Publish directory: `frontend/build`
3. **Add environment variables** in Netlify settings
4. **Deploy automatically** on every push

### Manual Deployment

#### Build for Production
```bash
cd frontend
npm run build
```

#### Deploy Build Folder
- Upload `frontend/build` folder to your hosting service
- Configure environment variables on your hosting platform

## 🔒 Security Notes

- **API Key Protection**: Never commit `.env` file to version control
- **Environment Variables**: Use production environment variables for deployment
- **HTTPS**: Always use HTTPS in production
- **Input Validation**: All user inputs are processed and sanitized

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature-name`
3. Commit changes: `git commit -m 'Add feature'`
4. Push to branch: `git push origin feature-name`
5. Submit a pull request

## 📝 License

This project is created by **Sanyam Suyal** for drone emergency assistance and safety education.

## 📞 Support

For technical support or questions:
- Create an issue in the repository
- Check the troubleshooting section above
- Review the error console in your browser

## 🌟 Acknowledgments

- **Together AI** for providing the Mistral 7B model
- **React Team** for the amazing framework
- **Indian Emergency Services** for the comprehensive helpline system
- **Drone Safety Organizations** for safety protocols and guidelines

---

**⚡ AeroGuardian AI - Protecting Lives Through Advanced Technology ⚡**

*Stay safe, stay protected, stay informed.*
