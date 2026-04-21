TB Learning Log: Initial Commit & Git Sync
Date: 2026-04-21

What I was trying to do
Establish the initial repository structure for Project TB and sync local files with GitHub.

The problem

Had duplicate folders with case-sensitive naming conflicts (TechBridge vs tech-bridge).

Ran into a fatal: refusing to merge unrelated histories error after creating files on GitHub manually.

Encountered a Merge Conflict in index.html.

What I tried

Used ls -la to find the hidden .git folder.

Used rm -rf to delete the ghost folder from the home directory.

Ran git pull origin main --allow-unrelated-histories to force a sync.

Used the VS Code Source Control panel to "Accept Incoming Change" and resolve the conflict.

What I learned

The Pilot Rule: Never rename or move folders manually in Windows Explorer while Git is tracking them; use the IDE or git mv.

Sync First: Always clone the repo first before adding local files to avoid "unrelated histories."

Bash Safety: You can't delete a folder while you are standing inside it (cd .. first).

What I’ll try next

Commit 3 (Environment): Set up the project structure (folders for CSS/JS).

Protocol: Use the Focus Flight app and the Park It! protocol to document the state of the code before shutting down.
