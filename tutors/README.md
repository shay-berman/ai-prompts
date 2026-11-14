# AI Private Tutor Framework

Reusable, voice-first tutoring instructions for ChatGPT Projects.

## Quick start
1. Create a ChatGPT Project called **English Tutor**.
2. Copy [project-instructions.md](templates/project-instructions.md) into its Project Instructions.
3. Optionally add school materials and a private student profile **inside the Project**, not GitHub.
4. Start voice or text practice. The tutor will ask one question at a time.
5. Request a short written summary at the end of each lesson.

## Files
- [Tutor Core](core/tutor-core.md): subject-independent teaching behavior
- [English module](subjects/english.md): English-specific practice
- [Paste-ready Project Instructions](templates/project-instructions.md): standalone combined prompt
- [Student profile template](templates/student-profile.example.md): optional blank profile
- [Setup example](examples/english-tutor-setup.md): usage guide

## Architecture
The core defines pedagogy; subject modules define domain-specific activities. Compose both into a standalone Project Instructions file. ChatGPT Projects **do not automatically import Markdown files from GitHub**.

## Limitations
Prompts cannot guarantee persistent progress storage, activate voice mode, or automatically display a written summary during voice mode. Use only accessible session history and saved summaries.

## Privacy
Never commit identifiable student data or completed profiles to this public repository.