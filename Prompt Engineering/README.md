# Prompt Engineering — Hack Invaders Workshop
Teacher: Jeff Huang

A short follow-along for the Prompt Engineering workshop at ACM Hack's Hack Invaders. Use this to write better prompts while building your retro game today.

## Resources

- [Slides](https://docs.google.com/presentation/d/1F6JWKR46O6s6GIzGG4HcYIBdKH9FvFDl8mPrpdlZf3I/edit?usp=sharing)

## Why Prompting Matters

A vague prompt gives you generic or wrong output. A specific, well-structured prompt gives you something usable. Knowing how to prompt is now a core programming skill.

## The 4 Parts of a Good Prompt

| Part | Purpose |
|------|---------|
| Role | Who the AI should act as |
| Task | What you want done |
| Context | Background info it needs |
| Format | How the answer should look |

Bad:
```
Explain machine learning
```

Good:
```
Explain machine learning to a high school student in 5 bullet points
with one real-world example.
```

## Common Mistakes

- Too vague
- Missing context
- No clear goal
- No output format
- Asking for too much at once


## Prompting Techniques

1. Start with clear context.
2. Break big tasks into small ones.
3. Specify the output format.
4. Refine after each response — don't restart.


## Game-Dev Examples

Bad:
```
Make me a video game.
Add enemies.
My game is broken.
```

Good:
```
Act as a beginner-friendly game developer. Build a 2D space-shooter
where the player moves left/right, shoots bullets, and dodges
descending aliens. Use one HTML file with <canvas> and vanilla JS.
List the main features first, then give the code.
```

```
Act as a debugging assistant. My player ship isn't moving on arrow
key press. Here's my input code: [paste]. List the likely problem,
the cause, and the fix.
```


## Watch Out For

- **Hallucinations** — confident-sounding but false output. Better prompts reduce this.
- **Leaking secrets** — never paste API keys into a chat. Use a `.env` file and add it to `.gitignore`.
- **Fact-checking** — verify function names, APIs, and statistics by actually running the code.


## Tools

Chatbots for planning: ChatGPT, Claude, Gemini.
AI in your IDE for coding: Cursor, Claude Code, Zed AI, Antigravity.

Typical flow: brainstorm in a chatbot, build in the IDE.


## Create a Plan First

Before letting the AI write code, write a short plan and feed it in. Then ask for one feature at a time.

```markdown
# Plan: Asteroid Dodger
- Player moves left/right with arrow keys
- Asteroids fall from the top
- Collision ends the game
- Score counter increases over time
```

Then prompt:
```
Here's my plan: [paste]. Implement only the first feature in a
single index.html file using <canvas> and vanilla JS. Add comments.
```

Tools that help you plan: Cursor Plan Mode, Amazon Kiro, Claude Code.


## Free Setup for Students

- Cursor Pro for Students — https://cursor.com/students
- Gemini for Students (CLI + Antigravity) — https://gemini.google/students/

Sign in with your `@ucla.edu` email.


**Exercise:** Rewrite `make a shooting game` using all four parts (Role, Task, Context, Format), then ask the AI to build only the first feature from a short plan.


## Takeaways

- Specific beats vague.
- Use Role, Task, Context, Format.
- Plan before you code.
- One feature at a time.
- Never paste secrets.
- Always test the output.

Good luck building.
