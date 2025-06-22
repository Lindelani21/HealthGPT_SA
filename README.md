# 🏥 HealthGPT SA - AI-Powered Healthcare Platform

![HealthGPT SA Banner](public/logo512.png)

> **A revolutionary AI-powered healthcare platform designed to make healthcare accessible, personalized, and engaging for South Africans.**

## 🌟 Features

### 📚 **Health Library**
- Doctor-reviewed articles
- Educational videos
- Condition information
- Saved articles functionality
- Trending health topics
![Health Library](public/health1.png)
![Article View](public/health3.png)
![Video Content](public/health4.png)
![Conditions Database](public/health2.png)

### 🎮 **Gamified Learning**
- Interactive health education games
- XP and badge reward system
- Community leaderboard
- Health knowledge challenges
![Games Overview](public/rewards1.png)
![Gameplay](public/rewards2.png)
![Badges](public/rewards3.png)
![Leaderboard](public/rewards4.png)

### 🏠 **Dashboard View**
- Personalized health metrics tracking
- Quick access to essential services
- Appointment reminders and health tips
![Dashboard](public/dashboard.png)

### 🗓️ **Appointments View**
- Clinic discovery and booking system
- Upcoming appointments tracking
- Video consultation options
![Appointments](public/appointment.png)
![Booking](public/booking.png)

### 🤖 **AI Assistant View**
- Medical image analysis
- Prescription reader
- Drug interaction checker
- Symptom severity assessment
- AI-powered medical chat
![AI Assistance](public/assistance.png)
![AI Assistance 2](public/assistance2.png)
![Scan Feature](public/scan.png)

### 👥 **Community View**
- Health-focused social feed
- Local health events
- Support groups
![Community](public/community.png)

### 🧠 **Mental Health View**
- Mood tracker
- Crisis support contacts
- Counselor booking
![Mental Health](public/mental1.png)
![Mental Health](public/mental2.png)

## 🛠️ Technical Implementation

### Health Library Components
```jsx
// Tab system for different content types
const tabs = [
  { id: 'articles', label: 'Articles', icon: MessageCircle },
  { id: 'videos', label: 'Videos', icon: Camera },
  { id: 'conditions', label: 'Conditions', icon: Heart }
];

// Article saving functionality
const handleSaveArticle = (id) => {
  setArticles(articles => articles.map(article =>
    article.id === id ? { ...article, saved: !article.saved } : article
  ));
};
