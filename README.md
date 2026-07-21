



Step-by-Step Implementation

1. Set up GitHub OAuthDecap requires an OAuth app so your content managers can log in with their GitHub credentials.
Go to your GitHub Developer Settings > OAuth Apps > New OAuth App.
Set Homepage URL to your production URL (e.g., https://yourdomain.com).
Set Authorization callback URL to https://yourdomain.com.

Application name
MispinoStore

Homepage URL
https://store.mispino.in

Authorization callback URL
https://store.mispino.in

-------------------------------------------
develop a react site on pc:
Step 1: Install Required Tools - Node.js, VS Code

Step 2: Create Your React Project - Folder/Open with Code/New Terminal
npm create vite@latest .
Javascript

Step 3: Install Dependencies and Start the Server
npm install
npm run dev
http://localhost:5173

Step 4: Edit Your Site
src folder - edit main.jsx
Edit the code inside it, save your file (Ctrl + S), and your web browser will automatically update

-------------------------------------------
Add React project to github

To add your local React project to GitHub, you will use Git to track your changes and push them to a remote repository.

1. Install Git and Sign In
2. Initialize Git in Your Project
Check status:
git status
Initialize (only run this if the previous step throws an error saying it is not a git repository):
git init
Stage files: Prepare all your files to be committed:
git add .
Commit changes: Save a snapshot of your current code locally:
git commit -m "Initial commit"

3. Create a New Repository on GitHub
Go to GitHub and log into your account.
Click the + icon in the top-right corner and select New repository.
Name your repository (e.g., my-react-site).
Leave "Initialize this repository with" checkboxes unchecked (do not add a README, .gitignore, or license, as Vite already created these).
Click Create repository.

# 1. Rename your default branch to main
git branch -M main

# 2. Link your local project to your GitHub repository
git remote add origin https://github.com/Inscribe/MispinoStore

# 3. Push your code to GitHub
git push -u origin main









References:
https://decapcms.org/docs/intro/

