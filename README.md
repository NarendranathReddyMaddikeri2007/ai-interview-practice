# AI Interview Practice

## Overview

**AI Interview Practice** is a next-generation web platform for software professionals to practice self-video interviews across various technologies (Java, Python, Java Testing, Python Testing, Frontend, Salesforce, and more). The platform leverages AI to analyze candidate responses—providing detailed feedback on confidence, English fluency, strengths, weaknesses, and overall performance through speech and facial analysis.

Candidates can select interview levels based on years of experience (e.g., 2, 4, 6 years) or opt for a general mode where questions progress from easy to hard. Admins can upload and manage questions, analyze candidate performance with visual charts, and manage users and groups.

---

## Features

- **Role-Based Access**
  - **Participant:** Practice interviews, receive AI feedback, track progress.
  - **Tech Admin:** Manage questions for specific technologies.
  - **Admin:** User management, question management, analytics.

- **Interview Practice**
  - Self-video interview sessions with real-time AI analysis.
  - Select technology and experience level or general mode.
  - Receive AI-generated summaries, ratings, and feedback on strong/weak areas, confidence, and fluency.

- **Question Management**
  - Admins upload, edit, and categorize questions by technology and difficulty.
  - Tag questions for group-based analysis.

- **Analytics & Reporting**
  - Visual charts for candidate and group performance.
  - Detailed breakdowns by technology, experience, and tags.

- **Scalable Microservices Architecture**
  - Spring Boot microservices with API Gateway, Service Registry, Central Config, and Auth Server.
  - Kafka for efficient video streaming and processing.

---

## Technology Stack

- **Frontend:** ReactJS
- **Backend:** Spring Boot (Microservices, Multithreaded)
  - API Gateway
  - Central Cloud Config
  - Service Registry (Eureka/Consul)
  - Auth Server (OAuth2/JWT)
  - Independent Microservices (User, Interview, Question, Analytics, AI Analysis, etc.)
  - Kafka (Video streaming and event-driven communication)
- **Database:** MySQL, MongoDB (for large unstructured data)
- **AI/ML Integration:** Speech and facial analysis for feedback (integrate with cloud AI services or custom models)
- **Deployment:** Docker, Kubernetes (optional for scaling)

---

## Getting Started

### Prerequisites

- Node.js & npm (for React frontend)
- Java 17+ (for Spring Boot backend)
- MySQL & MongoDB
- Kafka
- Docker (optional, for containerization)

### Installation

#### 1. Clone the Repository

```bash
git clone https://github.com/your-username/ai-interview-practice.git
cd ai-interview-practice
