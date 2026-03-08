# EduSign - AI-Powered Accessible Learning Platform

Mobile app making education accessible through automated Indonesian Sign Language (SIBI) synthesis and AI-generated quizzes.

**Used by stakeholders in academic competition**

## Problem Solved
Deaf students struggle to access video learning content. Manual SIBI translation is expensive and time-consuming.

## Key Features

### 1. Automated SIBI Video Synthesis
- YouTube link → Whisper AI transcription → morphological analysis → word-by-word SIBI clip matching → synchronized overlay
- Converts any Indonesian educational video into sign language automatically

### 2. AI Quiz Generation
- Groq API (GPT OSS 120B) generates 5 structured multiple-choice questions per video
- Automatic assessment for comprehension checking

### 3. Secure API Integration
- All Groq API calls routed through Google Cloud Functions
- API keys never exposed in Flutter client
- Production-grade security architecture

### 4. Authentication
- Google OAuth for seamless teacher/student login
- Role-based access (teacher vs student)

## Tech Stack
- **Frontend:** Flutter
- **AI Services:** Whisper AI (transcription), Groq API (quiz generation)
- **Backend:** Firebase, Google Cloud Functions
- **Auth:** Google OAuth

## Impact
- Used by stakeholders in academic competition
- Deployed production app with real users
- Demonstrates AI + mobile + cloud integration

## App Flow
```
1. Teacher uploads YouTube link
2. Whisper AI transcribes audio
3. System matches transcript to SIBI video clips
4. Synchronized SIBI video generated
5. Groq API generates comprehension quiz
6. Students watch + take quiz
```

## Team Project
Built as part of Software Engineering course (PPL 2) at Universitas Padjadjaran

## Security Highlight
Implemented serverless architecture (Google Cloud Functions) to protect API credentials - a production-ready security pattern for mobile apps integrating with LLMs.

---

**For detailed writeup:** [portfolio link if available]
