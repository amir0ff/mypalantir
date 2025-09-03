# 🔮 MyPalantir - A Gemini-Inspired AI Knowledge System
![Static Badge](https://img.shields.io/badge/Google-Gemini-%238E75B2?logo=googlegemini)

> **🚀 Quick Start:** This repository is a template for the MyPalantir system. Follow the steps below to create your own private, personalized version.

## 🏛️ Overview

MyPalantir replicates the organizational framework of Google's Gemini project, providing a structured approach for managing AI-generated content, conversation history, and custom AI personas (Gems).

## 🚀 Getting Started

### Step 1️⃣: Create Your Private Repository from this Template
Click the **"Use this template"** button at the top of this repository's page and select **"Create a new repository."**

On the creation page, give your new repository a name (e.g., `MyPalantir-Personal`) and, most importantly, set its visibility to **Private**. This will create a brand new, private copy of the system in your own account with a clean history, ready for your personal use.

### Step 2️⃣: Personalize Your System
Now that you have your own private copy, customize the template with your information:

1.  **Create Your Profile:** Rename `saved_info/example_user_profile.md` to `user_profile.md` and fill it out.
2.  **Customize Your Gems:** Explore the pre-built `gems/Career guide/`, `gems/Learning coach/`, and `gems/Writing editor/`. Add any reference materials to the `knowledge/` subfolder within each gem.
3.  **Clean Up:** Delete the example chat files in the `chats/` directory.

### Step 3️⃣: Start Your First Conversation
You're all set! To start a new chat, create a new file and use the prompt structure below. It tells the AI which persona, knowledge base, and user profile to load for the session.

**Example Starting Prompt:**

```yaml
# Session Context: Define the AI's environment, resources, and save location.
gem:
  persona: "@gems/Writing editor/writing_editor.mdc"
  knowledge: "@gems/Writing editor/knowledge/"
chat:
  save_to: "chats/writing_session_0/writing_session_0.md"
  attached_files: "@chats/writing_session_0/files/"
profile: "@saved_info/user_profile.md"

prompt: "Okay, I'm ready to start. I need to write a professional email to a potential client. Can you help me draft it? I want it to be clear, concise, and persuasive."
```

This structured prompt allows the AI to clearly understand its role, the knowledge it should use, your personal context, and the specific goals of the conversation before you even ask your first question.

## 📂 Project Structure

```
MyPalantir/
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

*MyPalantir - Your personal AI knowledge management system*
