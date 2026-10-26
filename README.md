<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:FF6B6B,35:FFA94D,70:4DABF7,100:845EF7&height=200&section=header&text=AI%20Interview%20Bot&fontSize=44&fontColor=ffffff&fontAlignY=36&animation=fadeIn&desc=Voice-based%20mock%20interviews%20with%20speech-to-text%20answers&descSize=16&descAlignY=58" width="100%"/>

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&color=845EF7&center=true&vCenter=true&width=700&lines=Pick+a+course+and+start+an+interview;Questions+are+read+aloud+to+you;Speak+your+answer+%E2%80%94+Whisper+transcribes+it;Admins+manage+courses+%26+questions" alt="Typing SVG"/>

<br/>

<img src="https://img.shields.io/badge/React%2018-61DAFB?style=for-the-badge&logo=react&logoColor=black" alt="React"/>
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript"/>
<img src="https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white" alt="Vite"/>
<img src="https://img.shields.io/badge/Tailwind%20CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white" alt="Tailwind CSS"/>
<img src="https://img.shields.io/badge/shadcn%2Fui-000000?style=for-the-badge&logo=shadcnui&logoColor=white" alt="shadcn/ui"/>
<img src="https://img.shields.io/badge/Supabase-3FCF8E?style=for-the-badge&logo=supabase&logoColor=white" alt="Supabase"/>
<img src="https://img.shields.io/badge/OpenAI%20Whisper-412991?style=for-the-badge&logo=openai&logoColor=white" alt="OpenAI Whisper"/>

<br/>

<img src="https://img.shields.io/badge/Status-Active-20C997?style=for-the-badge" alt="Status"/>
<img src="https://img.shields.io/github/stars/Annepuuday111/AI-Interview-Bot?style=for-the-badge&color=845EF7" alt="Stars"/>
<img src="https://img.shields.io/github/last-commit/Annepuuday111/AI-Interview-Bot?style=for-the-badge&color=4DABF7" alt="Last Commit"/>
<img src="https://img.shields.io/github/repo-size/Annepuuday111/AI-Interview-Bot?style=for-the-badge&color=FF6B6B" alt="Repo Size"/>

<br/><br/>

[About](#-about) • [Features](#-features) • [Tech Stack](#️-tech-stack) • [Architecture](#️-architecture) • [Getting Started](#-getting-started) • [Roadmap](#️-roadmap) • [Author](#-author)

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%">

## 📖 About

**AI Interview Bot** is a web app for practising spoken interviews. Admins build courses and question banks; students pick a course and sit a mock interview in the browser. Each question is read aloud, the student answers by voice with their camera on, and the recording is transcribed by **OpenAI Whisper** through a **Supabase Edge Function**. Answers are saved to the student's interview history.

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%">

## ✨ Features

| | Feature |
| :---: | :--- |
| 🔐 | **Supabase Auth** – email / password sign-up with a *Student* or *Admin* role, role-based redirect after login |
| 📚 | **Courses** – students browse courses and view course details before starting |
| 🎙️ | **Voice interview** – questions spoken with the browser Speech Synthesis API, answers recorded with `MediaRecorder` |
| 📹 | **Camera preview** during the interview |
| 📝 | **Speech-to-text** – audio sent to the `transcribe-audio` Edge Function (OpenAI `whisper-1`) |
| 🗂️ | **Interview history** – completed interviews per course with date and questions answered (transcripts stored in `result_summary`) |
| 🧑‍🏫 | **Admin dashboard** – counts of courses, questions and support queries |
| 🛠️ | **Manage courses & questions** – create, edit and delete courses; add and delete questions with difficulty (easy / medium / hard) and expected answers |
| 🛡️ | **Row Level Security** – students see only their own data, only admins can modify courses and questions |
| 💅 | Responsive UI built with Tailwind CSS and shadcn/ui (Radix) components |

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%">

## 🛠️ Tech Stack

<div align="center">

<img src="https://skillicons.dev/icons?i=react,ts,vite,tailwind,supabase,postgres&theme=light" alt="Tech icons"/>

</div>

| Layer | Technology |
| :--- | :--- |
| **Frontend** | ![React](https://img.shields.io/badge/React%2018-61DAFB?style=for-the-badge&logo=react&logoColor=black) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white) ![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white) ![React Router](https://img.shields.io/badge/React%20Router-CA4245?style=for-the-badge&logo=reactrouter&logoColor=white) |
| **UI** | ![Tailwind](https://img.shields.io/badge/Tailwind%20CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white) ![shadcn/ui](https://img.shields.io/badge/shadcn%2Fui-000000?style=for-the-badge&logo=shadcnui&logoColor=white) ![Radix UI](https://img.shields.io/badge/Radix%20UI-161618?style=for-the-badge&logo=radixui&logoColor=white) |
| **State & Forms** | ![TanStack Query](https://img.shields.io/badge/TanStack%20Query-FF4154?style=for-the-badge&logo=reactquery&logoColor=white) ![React Hook Form](https://img.shields.io/badge/React%20Hook%20Form-EC5990?style=for-the-badge&logo=reacthookform&logoColor=white) ![Zod](https://img.shields.io/badge/Zod-3E67B1?style=for-the-badge&logo=zod&logoColor=white) |
| **Backend** | ![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?style=for-the-badge&logo=supabase&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white) ![Deno](https://img.shields.io/badge/Edge%20Functions%20(Deno)-000000?style=for-the-badge&logo=deno&logoColor=white) |
| **AI** | ![OpenAI](https://img.shields.io/badge/OpenAI%20Whisper-412991?style=for-the-badge&logo=openai&logoColor=white) |

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%">

## 🏗️ Architecture

```text
React + Vite SPA
   │  @supabase/supabase-js
   ├──► Supabase Auth            (sign-up / login, role in user metadata)
   ├──► Supabase Postgres + RLS  (profiles, courses, questions, interviews, support_queries)
   └──► Edge Function  transcribe-audio  ──►  OpenAI Whisper (whisper-1)
```

### 📂 Project Structure

```text
AI-Interview-Bot/
├── public/
├── src/
│   ├── components/ui/          # shadcn/ui components
│   ├── hooks/
│   ├── integrations/supabase/  # Supabase client & generated types
│   ├── lib/
│   ├── pages/
│   │   ├── Index.tsx           # Landing page
│   │   ├── Auth.tsx            # Login / sign-up with role
│   │   ├── StudentDashboard.tsx
│   │   ├── Courses.tsx
│   │   ├── CourseDetails.tsx
│   │   ├── Interview.tsx       # Voice interview flow
│   │   ├── Interviews.tsx      # Interview history
│   │   ├── AdminDashboard.tsx
│   │   ├── ManageCourses.tsx
│   │   └── ManageQuestions.tsx
│   ├── App.tsx                 # Routes
│   └── main.tsx
├── supabase/
│   ├── functions/transcribe-audio/index.ts
│   ├── migrations/             # Tables, enum, RLS policies, triggers
│   └── config.toml
├── tailwind.config.ts
├── vite.config.ts
└── package.json
```

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%">

## 🚀 Getting Started

### Prerequisites

- Node.js 18+ and npm
- A [Supabase](https://supabase.com/) project and the [Supabase CLI](https://supabase.com/docs/guides/cli)
- An OpenAI API key (for Whisper transcription)

### Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/Annepuuday111/AI-Interview-Bot.git
   cd AI-Interview-Bot
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Configure environment** – create `.env` in the project root:
   ```env
   VITE_SUPABASE_URL=https://your-project-id.supabase.co
   VITE_SUPABASE_PUBLISHABLE_KEY=your_supabase_anon_key
   VITE_SUPABASE_PROJECT_ID=your-project-id
   ```

4. **Set up the database and Edge Function**
   ```bash
   supabase link --project-ref your-project-id
   supabase db push
   supabase secrets set OPENAI_API_KEY=your_openai_api_key
   supabase functions deploy transcribe-audio
   ```

5. **Run the app**
   ```bash
   npm run dev
   ```
   Then open the local URL printed by Vite. Allow microphone and camera access when starting an interview.

### Scripts

| Command | Description |
| :--- | :--- |
| `npm run dev` | Start the Vite dev server |
| `npm run build` | Production build |
| `npm run build:dev` | Development-mode build |
| `npm run preview` | Preview the production build |
| `npm run lint` | Run ESLint |

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%">

## 🗺️ Roadmap

- [x] Role-based auth with Supabase
- [x] Voice interviews with Whisper transcription
- [x] Admin course & question management
- [ ] AI scoring and feedback on answers
- [ ] Support-query page for students
- [ ] Progress analytics charts

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%">

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository
2. Create a branch: `git checkout -b feature/your-feature`
3. Commit your changes: `git commit -m "Add your feature"`
4. Push the branch: `git push origin feature/your-feature`
5. Open a Pull Request

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%">

## 👨‍💻 Author

<div align="center">

### Annepu Uday Kumar

<a href="https://github.com/Annepuuday111"><img src="https://img.shields.io/badge/GitHub-Annepuuday111-845EF7?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/></a>
<a href="https://annepuudaykumar.netlify.app"><img src="https://img.shields.io/badge/Portfolio-Visit-FF6B6B?style=for-the-badge&logo=netlify&logoColor=white" alt="Portfolio"/></a>

</div>

<br/>

<div align="center">⭐ If you like this project, give it a star!</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:845EF7,35:4DABF7,70:FFA94D,100:FF6B6B&height=120&section=footer" width="100%"/>
