# 👾 Hack Invaders

> A mini-hackathon where you take a retro classic and bring it into the future — powered by AI.

Welcome to **Hack Invaders**! Over the course of this event, you'll team up, pick a retro game, and revamp it using modern AI tools and techniques. Whether you're adding intelligent enemies, a global leaderboard, or multimodal controls, the goal is to breathe new life into old-school games.

---

## 🗂️ Workshops

Work through these workshops to build up your skills before (or during) the hackathon. Each one is self-contained and builds toward a fully AI-enhanced game.

---

### 🕹️ 1. Base Sample Game
**Start here.** Get the foundational game running locally so you have something to hack on.

- Set up the project and run the starter game
- Understand the game loop, input handling, and rendering
- Identify the hooks where you'll inject AI features

📁 [`/workshops/01-base-sample-game`](./workshops/01-base-sample-game)

---

### 💬 2. Prompt Engineering
**Learn to talk to AI effectively.** This workshop covers how to craft prompts that produce consistent, useful results in a game context.

- Understand prompt structure: system, user, and assistant roles
- Techniques: few-shot examples, chain-of-thought, structured output
- Apply prompts to generate game dialogue, enemy behavior descriptions, and level ideas

📁 [`/workshops/02-prompt-engineering`](./workshops/02-prompt-engineering)

---

### 🤖 3. AI in Video Games
**Bring intelligence to your game.** Go beyond scripted enemies and static content by integrating AI-driven behavior.

- Use LLMs to power dynamic NPC dialogue and decision-making
- Generate adaptive difficulty and procedural content
- Explore AI patterns: reactive agents, generative storytelling, and more

📁 [`/workshops/03-ai-in-video-games`](./workshops/03-ai-in-video-games)

---

### 🏆 4. Creating a Leaderboard
**Make it competitive.** Add a real-time leaderboard so players can compete across teams and sessions.

- Set up a backend to store and retrieve scores
- Display live rankings in your game UI
- Optionally: use AI to generate personalized taunts or congratulations based on rank

📁 [`/workshops/04-creating-a-leaderboard`](./workshops/04-creating-a-leaderboard)

---

### 🎙️ 5. Multimodal AI
**Go beyond text.** Use voice, images, and more to create richer, more expressive game experiences.

- Integrate image recognition, speech-to-text, or generative image APIs
- Control your game with your voice or react to what the camera sees
- Generate sprites, backgrounds, or sound effects using AI

📁 [`/workshops/05-multimodal-ai`](./workshops/05-multimodal-ai)

---

## 🚀 Getting Started

```bash
git clone https://github.com/your-org/hack-invaders.git
cd hack-invaders
# Follow setup instructions in /workshops/01-base-sample-game
```

---

## 📋 Hackathon Rules

- Teams of 1–4 people
- Must use at least one AI feature from the workshops
- Final submission includes: a playable game + a 2-minute demo
- Judging criteria: creativity, technical execution, and fun factor

---

## 🛠️ Tech Stack Suggestions

| Layer | Options |
|---|---|
| Game Engine | Pygame, Phaser.js, vanilla Canvas |
| AI / LLM | Claude API, OpenAI, Ollama |
| Leaderboard | Supabase, Firebase, simple REST API |
| Multimodal | Whisper, Claude Vision, ElevenLabs |

---

## 🤝 Contributing

Found a bug in a workshop? Want to add a bonus challenge? PRs are welcome! Check [`CONTRIBUTING.md`](./CONTRIBUTING.md) for guidelines.

---

## 📄 License

MIT — go build something awesome.

---

*Made with ❤️ for Hack Invaders participants. May your framerate be high and your bugs be few.*
