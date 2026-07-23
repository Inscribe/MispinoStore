



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
-------------------------------------------
Deploy the site using cloudflare worker

To deploy a React site built with Vite to Cloudflare, the recommended approach is using Cloudflare Pages, which integrates perfectly with your GitHub repository and utilizes the Cloudflare Workers infrastructure under the hood.
Here are the two ways to handle deployment: using the automatic GitHub integration dashboard or using the wrangler CLI directly.
Option A: The Automatic Git Method (Recommended)This approach connects Cloudflare directly to your GitHub repository so that every time you push code, your site automatically updates.Log into your Cloudflare Dashboard.Navigate to Workers & Pages in the left sidebar.Click Create Application > Select the Pages tab > Click Connect to Git.Authenticate your GitHub account and select your my-react-site repository.In the Set up builds and deployments section, use these exact settings:Framework preset: ViteBuild command: npm run buildBuild output directory: distClick Save and Deploy.Cloudflare will compile your project and provide a live production URL ending in .pages.dev.





-------------------------------------------
Hot Module Replacement (HMR)
This method allows you to use the built-in VS Code Source Control Panel without typing any commands. 

1. Save your file: Press Ctrl + S (Windows/Linux) or Cmd + S (Mac) to save your .js file changes.
2. Open Source Control: Click the Source Control icon (looks like a branching graph) on the left sidebar, or press Ctrl + Shift + G.
3. Stage the changes: Find your modified .js file under the Changes section and click the + (Plus) icon next to it to stage it.
4. Write a commit message: Type a descriptive message (e.g., Update script logic) into the text box at the top of the panel.
5. Commit the file: Click the Commit button (or the checkmark icon ✓) right above the text box.
6.Push the changes: Click the blue Sync Changes button, or click the ... (Three Dots) icon next to Source Control and select Push. 





Add WISIWYG Editor
1. TinyMCE
To install TinyMCE using npm, navigate to your project directory and run npm install tinymce in your terminal. “To install TinyMCE using NPM, you can run the following command: NPM npm install tinymce@^8” - TinyMCE Documentation📦 Installation OptionsDepending on your project setups and version requirements, you can choose from the following installation scripts:Latest stable version (v8): npm install tinymce@^8Previous version (v7): npm install tinymce@^7Premium plugins package: npm install tinymce-premium@^8.3🛠️ Framework WrappersIf you are using a frontend framework, you should also install the corresponding official wrapper alongside the core package:React: npm install @tinymce/tinymce-react “Navigate to the project directory and install @tinymce/tinymce-react.” - TinyMCE DocumentationAngular: npm install @tinymce/tinymce-angular “Navigate into the project directory and install tinymce-angular .” - TinyMCE DocumentationVue: npm install @tinymce/tinymce-vue




References:
https://decapcms.org/docs/intro/

