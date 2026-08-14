<div align="center">
  <h1>🎮 Game On Track</h1>
  <p><strong>A powerful, AI-driven application to help you track your game progress and finish your battle passes on time.</strong></p>
  
  [![Live Demo](https://img.shields.io/badge/Live_Demo-game--on--track.vercel.app-brightgreen?style=for-the-badge&logo=vercel)](https://game-on-track.vercel.app/)
</div>

<br />

Welcome to the public release repository for **Game On Track**! This repository serves as a showcase for the project, providing an overview of its features, architecture, and live deployment for those interested in the application or my work.

> **Note**: The source code for this project is maintained in a private repository to protect the proprietary backend implementations and secure configurations. This repository contains the public facing documentation and tracking of our public releases.

## ✨ Project Overview

Game On Track is a modern, responsive web application designed to solve the common problem of tracking multiple game seasons and battle passes. It intelligently calculates the required daily progress, visualizing whether a player is on track to complete their goals before the season ends.

### 🌟 Key Features

*   **🤖 AI-Powered Data Fetching:** Integrates with the **Groq API** (`groq/compound-mini`) to automatically fetch accurate start dates, end dates, total levels, and season names for any game.
*   **📊 Advanced Analytics & Velocity Tracking:** Calculates the exact "Levels per Day" (L/D) required to finish a pass on time, tracks pace status (On Track, Behind, Complete), and provides dynamic trajectory predictions based on actual progress.
*   **♻️ Recycle Bin & Data Safety:** Deleted games are securely moved to a 30-day retention Recycle Bin, offering users peace of mind and the ability to restore accidentally removed progress.
*   **📈 Interactive Data Visualization:** Features beautiful, interactive line charts comparing actual progress against the required pace over time.
*   **🔒 Secure Cloud Sync:** Implements **Firebase Auth** and **Firestore** for real-time, secure data synchronization across devices, including auto-retry and offline-aware capabilities.
*   **🎨 Premium UI/UX:** Built with a fully responsive, modern dark-mode aesthetic utilizing Inter, Space Grotesk, and Outfit typography. Includes drag-and-drop reordering, custom glowing color pickers, fluid micro-animations, and a highly scalable navigation sidebar to support massive game libraries seamlessly.

## 🛠️ Architecture & Tech Stack

This project was built with a focus on performance, security, and a premium user experience:

*   **Frontend**: Vanilla HTML/JS/CSS focusing on high performance without framework overhead, utilizing modern CSS features (glassmorphism, gradients) and responsive design principles.
*   **Backend / Serverless**: **Vercel Serverless Functions** are used to securely route AI requests, keeping API keys completely hidden from the client and handling rate limits with exponential backoff.
*   **Database & Auth**: **Firebase (Firestore + Authentication)** for secure user management and real-time database capabilities.
*   **AI Integration**: **Groq API** for lightning-fast inference to power the automatic data fetching feature.
*   **Security**: Strict Content-Security-Policy (CSP), server-side input sanitization, API rate limiting, and XSS protection.

## 🚀 Live Application

Experience the application yourself! No account required to try out the basic features:

**🔗 [game-on-track.vercel.app](https://game-on-track.vercel.app/)**

---

*Thank you for taking the time to check out my project! If you're a recruiter or hiring manager, I'd be happy to discuss the technical decisions, architecture, and private source code of this application in detail during an interview.*
