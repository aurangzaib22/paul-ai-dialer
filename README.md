# 📞 Paul AI Dialer

### AI-Powered Calling & Automation Platform

A modern, responsive frontend for managing AI-assisted outbound calling workflows, contact lists, voice settings, system prompts, and call performance.

[**🌐 Live Demo**](https://paul-ai-dialer.netlify.app/) · [**💻 Source Code**](https://github.com/aurangzaib22/paul-ai-dialer)

---

## 📖 Overview

**Paul AI Dialer** is a React and TypeScript web application for interacting with AI-assisted outbound calling services. It brings together contact uploads, call initiation, agent prompt configuration, voice management, call history, and performance monitoring in a user-friendly interface.

> **Project scope:** This repository contains the **frontend application**. Actual call placement, voice processing, recordings, transcripts, authentication APIs, and other server-side functionality depend on an external backend service, which is **not included** in this repository.

## ✨ Key Features

- **Outbound calling workflows:** Forms and API integration for initiating AI-assisted bulk calls and checking call status.
- **Contact management:** Contact upload interface and retrieval of saved contacts for call workflows.
- **Call analytics:** Dashboard views for call history, success status, metrics, and visual reporting.
- **Recordings & transcripts:** Interfaces for retrieving call recordings and conversation transcripts from the backend.
- **AI prompt customization:** Create, retrieve, and update agent prompts through API-connected settings.
- **Voice configuration:** Dedicated interfaces for agent voice selection and management.
- **Authentication flows:** Sign-in, registration, password recovery, and protected application routes.
- **State management & UI:** Redux Toolkit, responsive Tailwind CSS layouts, charts, animations, and toast notifications.
- **Calendar connection:** An API integration point for Google authorization.

## 🛠️ Tech Stack

| Area | Technologies |
| --- | --- |
| Frontend | React 19, TypeScript |
| Styling | Tailwind CSS 4, Framer Motion |
| State management | Redux Toolkit, React Redux |
| Routing | React Router |
| Forms | React Hook Form |
| API integration | Axios, REST APIs |
| Charts | Recharts |
| UI & notifications | Lucide React, React Icons, React Hot Toast, React Toastify |
| Build tooling | Vite 7 |

## 🚀 Getting Started

### Prerequisites

- Node.js and npm compatible with Vite 7
- Access to the backend API for authenticated calling and analytics features

### 1. Clone the repository

```bash
git clone https://github.com/aurangzaib22/paul-ai-dialer.git
cd paul-ai-dialer
```

### 2. Install dependencies

```bash
npm install
```

### 3. Configure the API URL

Create a `.env.local` file in the project root:

```dotenv
VITE_API_URL=https://your-backend-api.example.com
```

Replace the example with your actual backend base URL. The API client reads `VITE_API_URL` via `import.meta.env`.

> **Security:** Vite variables starting with `VITE_` are included in frontend bundles. Do not place API secrets, private tokens, or passwords in these variables. The source archive includes a `.env` file; review it before publishing, and make sure no credentials are committed to Git history.

### 4. Start the development server

```bash
npm run dev
```

Open the local URL shown by Vite.

### 5. Build and preview

```bash
npm run build
npm run preview
```

### Other command

```bash
npm run lint
```

## 🗂️ Project Structure

```text
paul-ai-dialer/
├── public/                 # Public images and static files
├── src/
│   ├── api/                # Authentication, call, voice, and dashboard API clients
│   ├── assets/             # Images, icons, and video assets
│   ├── components/         # Shared layout and landing-page components
│   ├── interfaces/         # TypeScript request and response types
│   ├── layout/             # Application layout
│   ├── pages/              # Dashboard, call form, prompts, uploads, voices, auth
│   ├── routes/             # Public and protected route wrappers
│   ├── store/              # Redux store and feature slices
│   ├── App.tsx             # App routes
│   └── main.tsx            # React entry point
├── package.json
└── vite.config.ts
```

## 🔐 Authentication & API Integrations

The app uses API client modules for authentication, call operations, contact uploads, prompt management, voice settings, and dashboard data. Protected routes require an authenticated session, and an Axios response interceptor handles unauthorized responses.

Features that request live call data, agent configuration, or recordings require a functioning backend and, where applicable, a valid account. The repository alone does not run an AI calling engine.

## 🌐 Live Application

**Live Demo:** https://paul-ai-dialer.netlify.app/

**GitHub Repository:** https://github.com/aurangzaib22/paul-ai-dialer

---

**Paul AI Dialer** · React · TypeScript · Redux Toolkit · AI-Assisted Calling Interfaces
