# Dentora — Dental Healthcare Chatbot

Dentora is a responsive dental healthcare assistant built with React, TypeScript,
Vite, and Tailwind CSS. It provides preliminary dental guidance, appointment
booking, and a simple daily oral-care checklist.

## Features

- Responsive dashboard with desktop and mobile navigation
- Home page with quick access to major features
- Dental assistant with symptom prompts and chat-style messages
- Dentist, date, and time selection
- Appointment confirmation and modification
- Interactive oral-health checklist
- Urgent-care conversation shortcut
- Privacy and medical-guidance notices

> Dentora provides general educational guidance only. It is not a substitute
> for diagnosis or treatment from a qualified dental professional.

## Technology Stack

- React 19
- TypeScript
- Vite 8
- Tailwind CSS 4
- Custom SVG icons

## Project Structure

```text
dentora/
├── public/
│   └── favicon.svg
├── src/
│   ├── App.tsx          # Application UI, state, and interactions
│   ├── index.css        # Tailwind import and global styles
│   ├── main.tsx         # React entry point
│   └── vite-env.d.ts    # Vite TypeScript declarations
├── index.html           # HTML entry point
├── package.json         # Dependencies and scripts
├── pnpm-lock.yaml       # Reproducible dependency versions
├── tsconfig.json        # TypeScript configuration
└── vite.config.ts       # Vite and Tailwind configuration
```

## Run Locally

### Requirements

- Node.js 22 or newer
- pnpm 10 or newer

### Commands

```bash
pnpm install
pnpm dev
```

Open the local URL printed by Vite in the terminal.

## Production Build

```bash
pnpm build
```

The optimized application is generated in the `dist` directory.

## Main Source Code

The complete interface and functionality are implemented in `src/App.tsx`.
Global styling is located in `src/index.css`, and React is mounted from
`src/main.tsx`.

## Suggested Demonstration Flow

1. Open **Home** and explain the three main modules.
2. Open **Dental Assistant**, select a symptom prompt, and send the message.
3. Toggle an item in the **Smile checklist**.
4. Open **Appointments**, choose a dentist, date, and time.
5. Confirm and then modify the appointment.

## Current Scope

This is a front-end academic prototype. Chat messages and appointments are held
in browser memory and reset when the page reloads. A production version could
add a backend database, authentication, dentist availability APIs, and a
clinically reviewed conversational AI service.
