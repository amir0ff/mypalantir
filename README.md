# 🔮 MyPalantir - A Gemini-Inspired AI Knowledge System (Antigravity Edition)
![Static Badge](https://img.shields.io/badge/Google-Gemini-%238E75B2?logo=googlegemini)
![Static Badge](https://img.shields.io/badge/Antigravity-IDE-%232377d5?logo=google)

> **🛸 Not using Antigravity?** Check out the **[Cursor Edition](https://github.com/amir0ff/mypalantir)** for the standard implementation.

## 🏛️ Overview

MyPalantir replicates the organizational framework of Google's Gemini project, providing a structured approach for managing AI-generated content, conversation history, and custom AI personas (Gems). 

**Version 3.0** is optimized for Gemini 3.0 models, featuring **Agentic Reasoning**, built-in psychological and pedagogical frameworks (**ACT, CBT, Socratic Method**), and **Automatic Context Ingestion**.

## 🚀 Getting Started

### Step 1️⃣: Create Your Private Repository from this Template
Click the **"Use this template"** button at the top of this repository's page and select **"Create a new repository."**

On the creation page, give your new repository a name (e.g., `MyPalantir-Personal`) and, most importantly, set its visibility to **Private**. This will create a brand new, private copy of the system in your own account with a clean history, ready for your personal use.

**Then, open this new repository in Antigravity.**

### Step 2️⃣: Personalize Your System
1.  **Create Your Profile:** Rename `saved_info/example_user_profile.md` to `user_profile.md` and fill it out.
2.  **Customize Your Gems:** Explore the pre-built `gems/Career guide/`, `gems/Learning coach/`, and `gems/Writing editor/`. Add any reference materials to the `knowledge/` subfolder within each gem.

### Step 3️⃣: Run the Context Workflow
To act as a persistent AI assistant, simply run the workflow:

> **"Run the load gem workflow"**

I will then:
1.  List your available Gems (e.g., "Career guide", "Writing editor").
2.  Ask you to choose one.
3.  **Automatically load** that persona and your user profile into the chat.

### Step 4️⃣: Start a New Chat
If you want to organize your conversation (just like the original MyPalantir), simply ask me to set it up:

> **"Start a new chat session for [Topic Name]"**

I will automatically:
1.  Create `chats/[Topic Name]/`
2.  Create the markdown file `chats/[Topic Name]/[Topic Name].md`
3.  Set the context so we can save our progress there.

*No complex YAML prompts required—just ask!*

## 📂 Project Structure

```
MyPalantir/
├── .agent/workflows/               # ⚡ AUTOMATION WORKFLOWS (Antigravity Exclusive)
│   └── load_gem.md                 # The script that makes context loading free
├── .cursor/rules/
│   └── global_context.mdc          # Global rule for automatic identity loading (for Cursor users)
├── README.md                       # This file
├── chats/                          # Chat conversation history and context
│   ├── example_chat_0/             # Each chat is in its own directory
│   │   ├── example_chat_0.md       # The chat markdown file
│   │   └── files/                  # Optional attached files for this chat
│   │       └── example_file.txt
│   └── example_chat_1/
│       └── example_chat_1.md
├── gems/                           # Core knowledge modules and AI personas
│   ├── Career guide/
│   │   └── career_guide.mdc        # Strategic career coach (v3.0)
│   ├── Learning coach/
│   │   └── learning_coach.mdc      # Socratic teaching persona (v3.0)
│   └── Writing editor/
│       ├── writing_editor.mdc      # Style-conscious senior editor (v3.0)
│       └── knowledge/              # Optional knowledge for this gem
│           └── Book.txt            # Example knowledge file
└── saved_info/                     # User account and profile information
    └── user_profile.md             # Your personalized profile
```

## 🗺️ Directory Purposes

### 📁 `/chats`
Contains detailed conversation history. In Version 3.0, any chat in this directory **automatically reads your identity** from `user_profile.md` via the global system rules (if using Cursor) or the workflow (if using Antigravity).

**Template Files:**
- `example_chat_0/` - A template directory for a new conversation, including an example `files/` folder.
- `example_chat_1/` - A template directory for a continuing conversation.

### 📁 `/gems`
Houses specialized AI personas (Gems). Version 3.0 Gems are powered by **Agentic Reasoning** and **Automatic Expertise Ingestion**. Each gem is a generic template that remains private until "plugged in" to your data.

**Template Gems:**
-   💼 **Career guide** - Strategic coach for planning, CV reviews, and interview prep.
-   📖 **Learning coach** - Socratic tutor that facilitates understanding through "Productive Struggle."
-   📝 **Writing editor** - Style-conscious senior editor.

### 📁 `/saved_info`
Stores persistent user information, preferences, and background context. This ensures AI interactions remain personalized and contextually aware.

**Template Files:**
- `user_profile.md` - Your personal user profile.

## 🗃️ File Format Guidelines

- **Chats**: Use `.md` format for conversation history and context
- **Gems**: Use `.mdc` format for Cursor IDE rules and AI personas
- **Saved Info**: Use `.md` format for user profiles and preferences
- **Knowledge**: Use appropriate formats (`.txt`, `.md`, `.pdf`, etc.) for reference materials

---

*MyPalantir - Your personal AI knowledge management system*
