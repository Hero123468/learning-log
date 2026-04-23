# Date: 2026-04-22

## What I was trying to do
Establish the initial repository structure for Project TB, initialize the Node.js environment, and install the session-recording dependency.

## The problem

Had duplicate folders with case-sensitive naming conflicts (TechBridge vs tech-bridge).

Ran into a fatal: refusing to merge unrelated histories error after creating files on GitHub manually.

Encountered a Merge Conflict in index.html.

New: Discovered the project was missing a package.json, preventing proper library installation.

New: node_modules was showing up in the "to-be-committed" list (too heavy for GitHub).

## What I tried

Used ls -la to find the hidden .git folder.

Used rm -rf to delete the ghost folder from the home directory.

Ran git pull origin main --allow-unrelated-histories to force a sync.

Used the VS Code Source Control panel to "Accept Incoming Change" to resolve the conflict.

New: Ran npm init -y to create the project "Passport" (package.json).

New: Created a .gitignore file and added node_modules/ to filter out heavy files.

New: Used git rm -r --cached . to reset Git's memory so it would respect the new ignore rules.

## What I learned

The Pilot Rule: Never rename or move folders manually in Windows Explorer while Git is tracking them; use the IDE or git mv.

Sync First: Always clone the repo first before adding local files to avoid "unrelated histories."

Bash Safety: You can't delete a folder while you are standing inside it (cd .. first).

The Cargo Rule: Never push node_modules to the cloud; always use a .gitignore to keep the flight light.

Initialization: Every professional web app needs a package.json before you start installing tools like rrweb.

## What I'll try next
SessionLog Schema: Define the MongoDB model to store the JSON data chunks.

Jules Training: Watch a tutorial or review documentation on the GitHub integration before the next flight.

Protocol: Continue using the Park It! protocol to ensure the tech-bridge repository stays clean and synced.
