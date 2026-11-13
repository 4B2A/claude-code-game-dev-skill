# 🎮 Claude Code: Game Dev Skill

A modular, engine-agnostic **Claude Code Skill** that turns your AI assistant into a structured Game Director and multi-agent development studio. Compatible with **Unity, Godot, Unreal, Phaser, Three.js**, and more.

## ✨ Key Features
* **3-Phase Production Pipeline:** Prevents spaghetti code by enforcing a strict *MVP -> Asset Integration -> Juice & UI* workflow.
* **Human-in-the-Loop Checkpoints:** Pauses after each phase to report progress and wait for your approval before moving forward.
* **Auto Engine Detection:** Scans your project directory to identify the game engine and applies its specific best practices.
* **Studio Subagent Roles:** Orchestrates specialized roles (*Coder*, *Tester*, *Juice Team*) for clean architecture, QA testing, and high game-feel.
* **Prohibiting Slop Code.

## 🚀 Installation

### Global Setup (All Projects)
```bash
git clone https://github.com/4B2A/claude-code-game-dev-skill
mkdir -p ~/.claude/skills
cp -r claude-code-game-dev-skill/skills/game-dev ~/.claude/skills/
```

### Project-Specific Setup
```bash
mkdir -p .claude/skills
cp -r claude-code-game-dev-skill/skills/game-dev .claude/skills/
```

## 💡 Usage
Launch Claude Code in your game project folder and describe your idea:

> *"I want to build a 2D top-down roguelike in Godot."*

## 🤝 Contributing
Contributions, issues, and feature requests are welcome! Feel free to open a PR.

## 📄 License
Distributed under the [MIT License](LICENSE).
