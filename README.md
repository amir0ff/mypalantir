# 🔮 MyPalantir - A Gemini-Inspired AI Knowledge System (Antigravity Edition)
![Static Badge](https://img.shields.io/badge/Google-Gemini-%238E75B2?logo=googlegemini)
![Static Badge](https://img.shields.io/badge/Antigravity-IDE-%232377d5?logo=google)

## 🏛️ Overview

MyPalantir replicates the organizational framework of Google's Gemini project, providing a structured approach for managing AI-generated content, conversation history, and custom AI personas (Gems). 

## 🚀 Getting Started

### Step 1️⃣: Create Your Private Repository from this Template
Click the **"Use this template"** button at the top of this repository's page and select **"Create a new repository."**

On the creation page, give your new repository a name (e.g., `MyPalantir-Personal`) and, most importantly, set its visibility to **Private**. This will create a brand new, private copy of the system in your own account with a clean history, ready for your personal use.

**Then, open this new repository in Antigravity.**

### Step 2️⃣: Personalize Your System
1.  **Create Your Profile:** Edit `saved_info/user_profile.md` with your details.
2.  **Customize Your Gems:** Explore the pre-built `gems/` folder. Add any reference materials to the `knowledge/` subfolder within each gem.

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
│   │   └── career_guide.mdc        # High-quality career coaching persona
│   ├── Learning coach/
│   │   └── learning_coach.mdc      # Persona to help learn new topics
│   └── Writing editor/
│       ├── writing_editor.mdc      # Persona to help you improve your writing
│       └── knowledge/              # Optional knowledge for this gem
│           └── Book.txt            # Example knowledge file
└── saved_info/                     # User account and profile information
    └── example_user_profile.md     # Template user profile
```

## 🗺️ Directory Purposes

### 📁 `/chats`
Contains detailed conversation history. Each chat is organized into its own directory, which holds the markdown conversation file and an optional `files/` subfolder for any relevant attachments like documents, images, or data files. This keeps each conversation and its related materials neatly bundled together.

**Template Files:**
- `example_chat_0/` - A template directory for a new conversation, including an example `files/` folder.
- `example_chat_1/` - A template directory for a continuing conversation.

### 📁 `/gems`
Houses specialized AI personas (Gems). Each gem is contained within its own directory, which holds the `.mdc` persona file and an optional `knowledge/` subfolder for relevant reference materials.

**Template Gems:**
-   💼 **Career guide** - Unlock your career potential. Get a detailed plan to refine your skills and achieve your career goals.
-   📖 **Learning coach** - Here to help you learn and practice new concepts. Tell me what you'd like to learn, and I'll help you get started.
-   📝 **Writing editor** - Elevate your writing. Get clear, constructive feedback, from grammar to structure.

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

*MyPalantir - Your personal, free AI knowledge management system*
