# 🔮 MyPalantir - A Gemini-Inspired AI Knowledge System (Cursor Edition)
![Static Badge](https://img.shields.io/badge/Google-Gemini-%238E75B2?logo=googlegemini)
![Static Badge](https://img.shields.io/badge/Cursor-IDE-black?logo=cursor&logoColor=white)

> **🛸 Antigravity User?** Check out the **[Antigravity Edition](https://github.com/amir0ff/mypalantir/tree/antigravity)** for a free, workflow-based alternative.

## 🏛️ Overview

MyPalantir replicates the organizational framework of Google's Gemini project, providing a structured approach for managing AI-generated content, conversation history, and custom AI personas (Gems). 

**Version 3.0** is optimized for Gemini 3.0 models, featuring **Agentic Reasoning**, built-in psychological and pedagogical frameworks (**ACT, CBT, Socratic Method**), and **Automatic Context Ingestion**.

## 🚀 Getting Started

### Step 1️⃣: Create Your Private Repository from this Template
Click the **"Use this template"** button at the top of this repository's page and select **"Create a new repository."**

On the creation page, give your new repository a name (e.g., `MyPalantir-Personal`) and, most importantly, set its visibility to **Private**. This will create a brand new, private copy of the system in your own account with a clean history, ready for your personal use.

### Step 2️⃣: Personalize Your System
Now that you have your own private copy, customize the template with your information:

1.  **Create Your Profile:** Rename `saved_info/example_user_profile.md` to `user_profile.md` and fill it out.
2.  **Customize Your Gems:** Explore the pre-built `gems/Career guide/`, `gems/Learning coach/`, and `gems/Writing editor/`. Add any reference materials to the `knowledge/` subfolder within each gem.
3.  **Clean Up:** Delete the example chat files in the `chats/` directory.

### Step 3️⃣: Start or Resume a Conversation
You're all set! To start a new chat, you can either create a markdown file yourself or simply ask the AI: **"Start a new chat session for [Topic] using the [Gem Name] persona."**

**The AI will automatically:**
1. Create a new directory and file in the `chats/` folder.
2. Insert the **Persona Anchor** header.
3. Load your identity and the Gem's expertise.

**Manual Setup Example:**
If you prefer to create the file yourself, use this structure at the top of your `.md` file:

```yaml
---
gem: "@gems/Writing editor/writing_editor.mdc"
---

# [Session Title]
prompt: "Okay, I'm ready to start. Can you help me analyze this decision?"
```

**Resuming a Session:**
Simply open any existing chat file and use the **Cursor Chat (Ctrl+L)**. Because the YAML anchor is at the top of the file, the AI will automatically resume with the correct persona and your personal context.

## 📂 Project Structure

```
MyPalantir/
├── .cursor/rules/
│   └── global_context.mdc          # Global rule for automatic identity loading
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
│   │   └── career_guide.mdc        # Strategic career coach
│   ├── Learning coach/
│   │   └── learning_coach.mdc      # Socratic teaching persona
│   └── Writing editor/
│       ├── writing_editor.mdc      # Style-conscious senior editor
│       └── knowledge/              # Optional knowledge for this gem
│           └── Book.txt            # Example knowledge file
└── saved_info/                     # User account and profile information
    └── example_user_profile.md     # Template user profile
```

## 🗺️ Directory Purposes

### 📁 `/chats`
Contains detailed conversation history. In Version 3.0, any chat in this directory **automatically reads your identity** from `user_profile.md` via the global system rules. Each chat remains organized into its own directory for bundling related materials neatly.

**Template Files:**
- `example_chat_0/` - A template directory for a new conversation, including an example `files/` folder.
- `example_chat_1/` - A template directory for a continuing conversation.

### 📁 `/gems`
Houses specialized AI personas (Gems). Version 3.0 Gems are powered by **Agentic Reasoning** and **Automatic Expertise Ingestion** (they automatically read their own `knowledge/` subfolders). Each gem is a generic template that remains private until "plugged in" to your data.

**Template Gems:**
-   💼 **Career guide** - Strategic coach for planning, CV reviews, and interview prep.
-   📖 **Learning coach** - Socratic tutor that facilitates understanding through "Productive Struggle."
-   📝 **Writing editor** - Style-conscious editor with voice mapping and cross-cultural nuance analysis.

### 📁 `/saved_info`
Stores persistent user information, preferences, and background context. This ensures AI interactions remain personalized and contextually aware.

**Template Files:**
- `example_user_profile.md` - Template for creating your personal user profile.

## 🗃️ File Format Guidelines

- **Chats**: Use `.md` format for conversation history and context
- **Gems**: Use `.mdc` format for Cursor IDE rules and AI personas
- **Saved Info**: Use `.md` format for user profiles and preferences
- **Knowledge**: Use appropriate formats (`.txt`, `.md`, `.pdf`, etc.) for reference materials

---

*MyPalantir - Your personal AI knowledge management system*
