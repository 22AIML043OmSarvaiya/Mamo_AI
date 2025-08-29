# 🏥 Mamo Health AI - Your AI-Powered Health Companion

<div align="center">

![Mamo Health AI](https://img.shields.io/badge/Health-AI%20App-blue?style=for-the-badge&logo=heart)
![React](https://img.shields.io/badge/React-18.0.0-blue?style=for-the-badge&logo=react)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-CSS-38B2AC?style=for-the-badge&logo=tailwind-css)
![Gemini AI](https://img.shields.io/badge/Gemini-AI%20Powered-orange?style=for-the-badge&logo=google)

**A Professional, Feature-Rich AI Health Application for University-Level Evaluation**

[🚀 Live Demo](#) • [📱 Features](#-features) • [🛠️ Tech Stack](#-tech-stack) • [🚀 Getting Started](#-getting-started)

</div>

---

## ✨ **Project Overview**

**Mamo Health AI** is a comprehensive, AI-powered health application that combines cutting-edge technology with beautiful, responsive design. Built for university-level evaluation, this project demonstrates advanced React development, AI integration, and modern UI/UX principles.

### 🎯 **Key Highlights**
- **🤖 AI-Powered Health Analysis** using Google Gemini API
- **📱 Fully Responsive Design** for all devices (Mobile, Tablet, Desktop)
- **🎨 Modern UI/UX** with beautiful animations and gradients
- **🔒 Professional Architecture** with React Context and modern hooks
- **📊 Interactive Charts** and data visualization
- **🌐 Multi-language Support** ready for international users

---

## 🚀 **Features**

### 🔥 **Core Features (Must-Have for 4th Year Project)**

| Feature | Description | Status |
|---------|-------------|---------|
| 🧠 **AI Symptom Checker** | AI analyzes symptoms and suggests causes & next steps | ✅ Complete |
| 💬 **Health Chatbot** | AI answers health queries in natural language | ✅ Complete |
| 🥗 **Diet & Nutrition** | AI recommends personalized diet plans | ✅ Complete |
| 🏃 **Fitness Tracking** | Track steps, sleep, calories with AI insights | ✅ Complete |
| 🚨 **Emergency Assistance** | Quick access to emergency services & hospitals | ✅ Complete |

### ⭐ **Advanced Features (Viva Impressors)**

| Feature | Description | Status |
|---------|-------------|---------|
| 🎯 **AI Risk Prediction** | Predicts risks for Diabetes, Heart Disease, Obesity | ✅ Complete |
| 📊 **Personalized Dashboard** | AI-powered health score with charts & progress | ✅ Complete |
| 💊 **Medicine Reminder** | AI reminders with interaction detection | ✅ Complete |
| 🖼️ **Image Analysis** | AI analyzes skin images for conditions | ✅ Complete |
| 🧘 **Mental Health Support** | AI stress relief & meditation guidance | ✅ Complete |
| 🌍 **Multi-language** | Support for English, Hindi, Gujarati, Spanish | ✅ Complete |

---

## 🛠️ **Tech Stack**

### **Frontend Framework**
- **React 18** - Latest React with modern hooks and features
- **React Router DOM** - Client-side routing
- **React Context API** - Global state management with useReducer

### **Styling & UI**
- **Tailwind CSS** - Utility-first CSS framework
- **Framer Motion** - Smooth animations and transitions
- **Lucide React** - Beautiful, consistent icons
- **Custom CSS** - Enhanced gradients, glass effects, and animations

### **Data Visualization**
- **Recharts** - Interactive charts and graphs
- **Responsive Design** - Mobile-first approach with breakpoints

### **AI Integration**
- **Google Gemini API** - Advanced AI health analysis
- **Custom AI Service** - Centralized AI interaction layer
- **Smart Prompts** - Structured, formatted AI responses

### **Development Tools**
- **Vite** - Fast build tool and development server
- **ESLint** - Code quality and consistency
- **Prettier** - Code formatting

---

## 🎨 **Design Features**

### **Modern UI Elements**
- ✨ **Glass Morphism** - Beautiful backdrop blur effects
- 🌈 **Gradient Backgrounds** - Eye-catching color schemes
- 🎭 **Smooth Animations** - Hover effects and transitions
- 📱 **Responsive Grid** - Adaptive layouts for all screen sizes

### **Enhanced User Experience**
- 🎯 **Interactive Elements** - Hover effects and micro-interactions
- 📊 **Data Visualization** - Charts, progress bars, and metrics
- 🔔 **Smart Notifications** - Toast messages and alerts
- 🎨 **Consistent Design Language** - Unified color palette and typography

---

## 🚀 **Getting Started**

### **Prerequisites**
- Node.js 16+ 
- npm or yarn
- Google Gemini API key

### **Installation**

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/mamo-health-ai.git
cd mamo-health-ai
```

2. **Install dependencies**
```bash
npm install
```

3. **Set up environment variables**
```bash
# Copy the example file
cp .env.example .env

# Add your Gemini API key
REACT_APP_GEMINI_API_KEY=your_gemini_api_key_here
```

4. **Start the development server**
```bash
npm start
```

5. **Open your browser**
Navigate to `http://localhost:3000`

### **Getting Your Gemini API Key**

1. Visit [Google AI Studio](https://makersuite.google.com/app/apikey)
2. Sign in with your Google account
3. Create a new API key
4. Copy the key to your `.env` file

---

## 📱 **Responsive Design**

### **Mobile-First Approach**
- 📱 **Mobile (320px+)** - Optimized touch interfaces
- 📱 **Tablet (768px+)** - Enhanced layouts with sidebars
- 💻 **Desktop (1024px+)** - Full-featured desktop experience

### **Breakpoint System**
```css
/* Mobile */
@media (max-width: 640px) { ... }

/* Tablet */
@media (min-width: 641px) and (max-width: 1024px) { ... }

/* Desktop */
@media (min-width: 1025px) { ... }
```

---

## 🤖 **AI Integration**

### **Gemini API Features**
- **Smart Health Analysis** - Context-aware symptom checking
- **Personalized Recommendations** - User-specific health advice
- **Multi-language Support** - AI responds in user's preferred language
- **Structured Responses** - Formatted, actionable health information

### **AI Service Architecture**
```javascript
// Centralized AI service
class AIService {
  async getAIResponse(prompt, context)
  async analyzeSymptoms(symptoms, userData)
  async predictHealthRisks(userData, lifestyleData)
  async getNutritionAdvice(userData, healthGoals)
  // ... more methods
}
```

---

## 📊 **Data Management**

### **State Management**
- **React Context** - Global application state
- **useReducer** - Complex state logic
- **Local Storage** - Persistent user data
- **Real-time Updates** - Live health metrics

### **Data Flow**
```
User Input → Context → AI Service → Gemini API → Response → UI Update
```

---

## 🎯 **Project Structure**

```
src/
├── components/          # React components
│   ├── Dashboard.js    # Main dashboard with charts
│   ├── Navbar.js       # Responsive navigation
│   ├── SymptomChecker.js # AI symptom analysis
│   ├── HealthChatbot.js # AI health chatbot
│   ├── RiskPrediction.js # Health risk assessment
│   ├── EmergencyAssistance.js # Emergency services
│   └── ...            # Other components
├── context/            # React context providers
│   └── HealthContext.js # Global state management
├── services/           # API and external services
│   └── aiService.js   # Gemini AI integration
├── styles/             # CSS and styling
│   └── index.css      # Enhanced Tailwind + custom CSS
└── App.js             # Main application component
```

---

## 🧪 **Testing & Quality**

### **Code Quality**
- **ESLint** - JavaScript/React linting
- **Prettier** - Code formatting
- **Modern React Patterns** - Hooks, Context, functional components

### **Performance**
- **Lazy Loading** - Component-level code splitting
- **Optimized Images** - WebP format support
- **Efficient Rendering** - React.memo and useMemo where appropriate

---

## 🌟 **Advanced Features**

### **AI-Powered Health Analysis**
- **Symptom Analysis** - Multi-category symptom checking
- **Risk Assessment** - Lifestyle-based health predictions
- **Nutrition Planning** - Personalized diet recommendations
- **Mental Health Support** - AI-guided wellness practices

### **Interactive Dashboard**
- **Health Score** - AI-calculated wellness metrics
- **Progress Tracking** - Visual health journey
- **Smart Notifications** - Context-aware health reminders
- **Data Visualization** - Charts and progress indicators

---

## 🚀 **Deployment**

### **Build for Production**
```bash
npm run build
```

### **Deploy Options**
- **Netlify** - Drag & drop deployment
- **Vercel** - Git-based deployment
- **GitHub Pages** - Static hosting
- **AWS S3** - Scalable cloud hosting

---

## 📚 **Documentation**

### **Component Documentation**
Each component includes:
- **Props Interface** - Type definitions
- **Usage Examples** - Implementation samples
- **Styling Guide** - CSS classes and customization
- **Responsive Behavior** - Breakpoint-specific features

### **API Documentation**
- **AI Service Methods** - Function signatures and parameters
- **Response Formats** - Data structure examples
- **Error Handling** - Common issues and solutions

---

## 🤝 **Contributing**

### **Development Guidelines**
1. **Fork the repository**
2. **Create a feature branch** (`git checkout -b feature/amazing-feature`)
3. **Commit your changes** (`git commit -m 'Add amazing feature'`)
4. **Push to the branch** (`git push origin feature/amazing-feature`)
5. **Open a Pull Request**

### **Code Standards**
- **ESLint** - Follow linting rules
- **Prettier** - Maintain code formatting
- **Component Structure** - Use established patterns
- **Responsive Design** - Mobile-first approach

---

## 📄 **License**

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

---

## 🙏 **Acknowledgments**

- **Google Gemini AI** - Advanced AI capabilities
- **React Team** - Amazing frontend framework
- **Tailwind CSS** - Utility-first styling
- **Open Source Community** - Inspiring tools and libraries

---

## 📞 **Support & Contact**

- **Project Link**: [https://github.com/yourusername/mamo-health-ai](https://github.com/yourusername/mamo-health-ai)
- **Issues**: [GitHub Issues](https://github.com/yourusername/mamo-health-ai/issues)
- **Discussions**: [GitHub Discussions](https://github.com/yourusername/mamo-health-ai/discussions)

---

<div align="center">

**Made with ❤️ for Health & Technology**

*This project demonstrates advanced React development, AI integration, and modern UI/UX principles suitable for university-level evaluation.*

[⬆️ Back to Top](#-mamo-health-ai---your-ai-powered-health-companion)

</div>
