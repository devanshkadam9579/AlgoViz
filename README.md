# 🔥 AlgoViz - Interactive DSA Visualization + AI Learning Platform

AlgoViz transforms how students learn Data Structures and Algorithms by combining **interactive visualizations** with **AI-powered explanations** and **handwritten-style notes**.

## 🎯 What AlgoViz Does

- **Visualizes** DSA concepts step-by-step with animations
- **Explains** algorithms using real-life stories (powered by Gemini AI)
- **Generates** handwritten-style memory notes for revision
- **Tracks** user progress with points and achievements
- **Provides** time & space complexity analysis
- **Allows** downloading notes as PDF/PNG for offline study

## ✨ New Features Added

### 🔐 Authentication System
- **Firebase Authentication** with email/password
- **User Registration** and secure login
- **Protected Routes** for authenticated users only

### 📊 User Dashboard
- **Progress Tracking** - Total questions solved and points earned
- **Achievement System** - Track completed algorithms
- **Learning Statistics** - Average scores and activity tracking
- **Visual Progress** - Beautiful stats cards and progress indicators

### 🎓 Enhanced Learning Experience
- **Improved Code Editor** - Better array parsing and syntax highlighting
- **Dynamic Visualizations** - Shows target values and search results
- **User Stats Integration** - Earn points for completing algorithms
- **Seamless Navigation** - Easy switching between dashboard and learning

## 🧩 Supported Algorithms (MVP)

### Search Algorithms
- **Linear Search** - Step-by-step element searching
- **Binary Search** - Efficient divide-and-conquer search

### Sorting Algorithms  
- **Merge Sort** - Recursive divide-and-merge visualization

### Data Structures
- **Stack** - LIFO operations (push, pop, overflow, underflow)
- **Queue** - FIFO operations (enqueue, dequeue)

### Techniques
- **Recursion** - Call stack visualization
- **Two Pointer** - Coordinated pointer movement
- **Sliding Window** - Efficient subarray processing

## 🏗️ Architecture

```
Frontend (React + Router)
├── Authentication (Firebase Auth)
├── User Dashboard (Progress Tracking)
├── Monaco Editor (Java code editor)
├── Canvas/SVG Animations
└── Protected Routes

Backend Services
├── Firebase Firestore (User Data)
├── Gemini AI Integration
└── Execution Step Processor

Data Flow
User Login → Dashboard → Learning Platform → Code → Visualization → AI Story → Notes → Points
```

## 🚀 Quick Start

### Prerequisites
- Node.js 18+
- npm or yarn
- Firebase project (optional for local development)

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/devanshkadam9579/AlgoViz.git
cd AlgoViz
```

2. **Install dependencies**
```bash
npm install
```

3. **Start development server**
```bash
npm run dev
```

4. **Open in browser**
   - Navigate to `http://localhost:3000`
   - Create an account or login to access the platform

## 🎨 Features

### 🔐 Authentication Flow
1. **Sign Up** - Create account with email/password
2. **Login** - Secure authentication with Firebase
3. **Dashboard** - View progress and statistics
4. **Learning** - Access interactive algorithms

### 📊 User Dashboard
- **Total Points** earned from completing algorithms
- **Questions Solved** counter with progress tracking
- **Algorithms Learned** - Unique concepts mastered
- **Current Streak** - Days of continuous learning
- **Recent Achievements** - Latest completed algorithms
- **Learning Statistics** - Detailed progress metrics

### 💻 Interactive Code Editor
- Monaco Editor with Java syntax highlighting
- Algorithm templates for quick start
- **Improved Array Parsing** - Supports multiple array declaration formats:
  ```java
  int[] arr = {1, 2, 3, 4, 5};
  int[] array = new int[]{10, 20, 30};
  {64, 34, 25, 12, 22, 11, 90}
  ```
- Real-time code editing and execution

### 🎬 Step-by-Step Visualization
- Canvas-based animations with smooth transitions
- **Interactive Controls** - Play, pause, step-through
- **Target Value Display** - Shows search targets clearly
- **Visual Feedback** - Green for found, red for not found
- **Progress Indicators** - Current step and total steps
- Visual complexity indicators (time/space)

### 🤖 AI-Powered Learning
- **Story Mode**: Real-life analogies for each algorithm
- **Visual Memory**: Describes what students just saw animated
- **Key Takeaways**: Memorable summary points
- **Structured Notes**: Complete study material generation

### 📝 Handwritten Notes
- Paper-like background with handwritten fonts
- **Highlighted Keywords** and important concepts
- **Memory Tricks** and mnemonics
- **Edge Cases** and important considerations
- **Complexity Analysis** breakdown
- **Export Options** - Download as PDF or PNG

### 🏆 Gamification
- **Points System** - Earn 10 points per algorithm completion
- **Progress Tracking** - Visual progress indicators
- **Achievement Badges** - For completed algorithms
- **Statistics Dashboard** - Comprehensive learning analytics

## 📁 Project Structure

```
src/
├── components/           # React components
│   ├── AlgorithmSelector.jsx    # Algorithm selection grid
│   ├── CodeEditor.jsx          # Monaco editor integration
│   ├── Dashboard.jsx           # User dashboard with stats
│   ├── HandwrittenNotes.jsx    # Notes with export functionality
│   ├── LearningPlatform.jsx    # Main learning interface
│   ├── Login.jsx              # Authentication login
│   ├── ProtectedRoute.jsx     # Route protection
│   ├── Signup.jsx             # User registration
│   ├── StoryMode.jsx          # AI-generated stories
│   └── Visualizer.jsx         # Canvas-based visualizations
├── contexts/            # React contexts
│   └── AuthContext.jsx        # Authentication state management
├── services/            # External services
│   └── geminiService.js       # Gemini AI integration
├── utils/               # Utility functions
│   ├── executionEngine.js     # Code processing and analysis
│   ├── visualizationRenderer.js # Canvas rendering engine
│   ├── codeTemplates.js       # Algorithm code templates
│   └── exportUtils.js         # PDF/PNG export functionality
├── firebase/            # Firebase configuration
│   └── config.js             # Firebase setup and initialization
└── App.jsx             # Main application with routing
```

## 🔧 Usage

### Getting Started
1. **Create Account** - Sign up with email and password
2. **View Dashboard** - See your learning progress and statistics
3. **Start Learning** - Click "Start Learning" to access algorithms

### Learning Flow
1. **Select Algorithm** - Choose from the algorithm grid
2. **Edit Code** - Modify the Java template or write your own
3. **Visualize** - Click "Visualize" to see the step-by-step animation
4. **Learn** - Read the AI-generated story and explanations
5. **Study** - Review the handwritten-style notes
6. **Export** - Download notes for offline revision
7. **Earn Points** - Get 10 points for each algorithm completion

## 🤖 AI Integration

AlgoViz uses Google's Gemini AI to generate:

1. **Story Mode**: 5-7 line real-life analogies
2. **Visual Memory**: Description of the animation
3. **Takeaways**: Key learning points
4. **Study Notes**: Structured revision material with:
   - Core concepts and key operations
   - Time and space complexity explanations
   - Memory tricks and mnemonics
   - Edge cases and important considerations

## 🔥 Key Improvements Made

### Code Editor Enhancements
- **Better Array Parsing** - Supports multiple Java array formats
- **Target Value Extraction** - Automatically finds search targets
- **Syntax Validation** - Real-time error checking

### Visualization Improvements
- **Dynamic Target Display** - Shows what you're searching for
- **Result Feedback** - Clear found/not found indicators
- **Step Descriptions** - Detailed explanations for each step
- **Interactive Controls** - Play, pause, and step-through animations

### User Experience
- **Authentication System** - Secure user accounts
- **Progress Tracking** - Points, achievements, and statistics
- **Responsive Design** - Works on all device sizes
- **Smooth Navigation** - Easy switching between sections

## 🚀 Deployment

### Local Development
```bash
npm run dev          # Start development server
npm run build        # Build for production
npm run preview      # Preview production build
```

### Production Deployment
1. **Build the application**: `npm run build`
2. **Deploy the `dist` folder** to your hosting service
3. **Configure Firebase** with your project settings
4. **Set up environment variables** for API keys

## 🔐 Firebase Setup

Replace the placeholder config in `src/firebase/config.js` with your Firebase project configuration:

```javascript
const firebaseConfig = {
  apiKey: "your-api-key",
  authDomain: "your-project.firebaseapp.com",
  projectId: "your-project-id",
  storageBucket: "your-project.appspot.com",
  messagingSenderId: "your-sender-id",
  appId: "your-app-id"
}
```

## 🎓 Educational Philosophy

AlgoViz is designed around the principle that **visualization + story + memory + gamification = mastery**.

- **Visual**: See how algorithms work step-by-step
- **Story**: Understand through real-life analogies  
- **Memory**: Remember with handwritten-style notes
- **Gamification**: Stay motivated with points and achievements
- **Practice**: Reinforce with interactive exploration

## 🚀 Future Enhancements

- **More Algorithms** (QuickSort, BFS, DFS, Dynamic Programming)
- **Multiple Languages** (Python, C++, JavaScript support)
- **Advanced Gamification** (Leaderboards, badges, challenges)
- **Social Features** (Share progress, collaborative learning)
- **Mobile App** (Native iOS/Android applications)
- **AI Tutoring** (Personalized learning recommendations)

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Google Gemini AI** for educational content generation
- **Firebase** for authentication and database services
- **Monaco Editor** for professional code editing experience
- **Canvas API** for smooth and interactive visualizations
- **React Ecosystem** for robust and scalable UI development

---

**AlgoViz** - Making algorithms unforgettable through visualization, stories, and gamification! 🧠✨🏆

## 📊 Stats at a Glance

- **8 Algorithms** supported with full visualization
- **4 Categories** - Search, Sort, Data Structures, Techniques  
- **AI-Powered** explanations and note generation
- **Gamified** learning with points and achievements
- **Export Ready** - PDF and PNG note downloads
- **Mobile Friendly** - Responsive design for all devices