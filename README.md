# 🐱 Pawmodoro

A web application that gamifies studying using the Pomodoro Technique combined with virtual pet care. Keep your focus sharp and your virtual cat happy!

## Table of Contents

- [Overview](#overview)
- [Features](#-features)
- [Project Structure](#-project-structure)
- [Installation](#-installation)
- [Usage Guide](#-usage-guide)
- [Contributing](#-contributing)
- [Team](#-team)
- [Credits](#-credits)
- [License](#-license)

## Overview

Pawmodoro is a productivity tool that helps you maintain focus while caring for virtual cats. By completing study intervals, you earn rewards to feed and interact with your virtual cats, creating a fun and motivating study environment.

This project was originally developed as a Java Swing application and has been migrated to a web stack using Spring Boot and Next.js.

### Why Pawmodoro?

- 🕒 Customizable study and break intervals
- 🐈 Virtual cat companions that respond to your study habits
- 📊 Track your progress and cat's well-being
- 🌐 Access from any device with a web browser

## ✨ Features

### 1. Timer Management

- Flexible study and break duration settings
- Visual progress tracking
- Customizable auto-start options

### 2. Virtual Cat Care System

- Feed and interact with virtual cats
- Monitor cat happiness and hunger levels
- Earn rewards through completed study sessions

### Features to Come

- Study session statistics
- Level progression system
- Music integration

## 🏗 Project Structure

```
pawmodoro/
├── pawmodoro-backend/    # Spring Boot backend
├── pawmodoro-web/       # Next.js frontend
└── README.md
```

## 📚 Installation

### Prerequisites

- Java 21 or higher
- Node.js 18 or higher
- Maven 3.8 or higher
- Git

### Cloning the Repository

1. Clone the main repository with its submodules:

```bash
git clone --recurse-submodules https://github.com/rachelkd/pawmodoro-web.git
cd pawmodoro-web
```

If you've already cloned the repository without submodules, initialize them with:

```bash
git submodule init
git submodule update
```

### Setting Up the Backend

1. Navigate to the backend directory:

```bash
cd pawmodoro-backend
```

2. Create a `application-local.properties` file in `src/main/resources` with your Supabase credentials:

```properties
supabase.url=your_supabase_url
supabase.key=your_supabase_anon_key
supabase.secret=your_supabase_service_role_key
```

3. Build and run the Spring Boot application:

```bash
./mvnw spring-boot:run
```

The backend will start on `http://localhost:8080`

### Setting Up the Frontend

1. Navigate to the frontend directory:

```bash
cd pawmodoro-web
```

2. Create a `.env.local` file with your Supabase credentials:

```env
NEXT_PUBLIC_SUPABASE_URL=your_supabase_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key
```

3. Install dependencies and run the development server:

```bash
npm install
npm run dev
```

The frontend will start on `http://localhost:3000`

## 📖 Usage Guide

1. **Getting Started**
   - Create an account or log in
   - Customize your study and break durations
   - Select your first virtual cat companion

2. **During Study Sessions**
   - Start the timer
   - Monitor your progress
   - Complete intervals to earn rewards

3. **Cat Care**
   - Feed your cat with earned rewards
   - Interact with your cat
   - Monitor happiness and hunger levels

## 🤝 Contributing

1. Create a new branch for your feature:
```bash
git checkout -b feature/your-feature-name
```

2. Make your changes and commit them:
```bash
git add .
git commit -m "Add your commit message"
```

3. Push to your branch:
```bash
git push origin feature/your-feature-name
```

4. Create a Pull Request from your branch to main.

For detailed contribution guidelines, please check our [Contributing Guide](CONTRIBUTING.md).

## 👥 Team

### Web Implementation Team

- [Rachel Deng (@rachelkd)](https://github.com/rachelkd)
- [Jeha Park (@jehapark)](https://github.com/jehapark)

### Original Java Swing Implementation Team

- [Allyssa Chiu (@chiually)](https://github.com/chiually)
- [Rachel Deng (@rachelkd)](https://github.com/rachelkd)
- [Jeha Park (@jehapark)](https://github.com/jehapark)
- [Manahill Sajid (@manahillsajid)](https://github.com/manahillsajid)
- [Jinny Yoo (@yhj050224)](https://github.com/yhj050224)

## 🎨 Credits

- Cat illustrations by [Natalia Kosheleva](https://www.istockphoto.com/portfolio/sicklemoon) on iStock
- Original Java Swing implementation: [pawmodoro](https://github.com/rachelkd/pawmodoro)

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details. 
