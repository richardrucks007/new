# nexusid-alert-ui

This is a Vite + React + TypeScript project scaffolded with shadcn/ui components.

This README includes instructions to:

- Initialize a Git repository and push to GitHub.
- Create a GitHub Actions workflow to build the project and upload the `dist` artifact.
- Host the built static site on DigitalOcean App Platform (or using Spaces + CDN).

Prerequisites
- Node.js (18+ recommended) and npm
- A GitHub account
- A DigitalOcean account

Quick local commands

1. Install dependencies
   npm install

2. Run dev server
   npm run dev

3. Build for production
   npm run build

4. Preview production build
   npm run preview

Create and push a GitHub repo (example)

1. Initialize git and commit
   git init
   git add .
   git commit -m "Initial commit"

2. Create a repo on GitHub (via web UI) and push
   git remote add origin git@github.com:<your-username>/<repo-name>.git
   git branch -M main
   git push -u origin main

CI: GitHub Actions (build + upload artifact)

The repository includes a workflow that builds the project on push to `main` and uploads the `dist` directory as an artifact. You can use this artifact in DigitalOcean or other deployment pipelines.

DigitalOcean hosting

Option A (App Platform):
- Connect your GitHub repo to DigitalOcean App Platform and select the `main` branch.
- Set the build command to `npm run build` and the output directory to `dist`.
- For a static site, choose the "Static Site" option. DigitalOcean will serve files from `dist`.

Option B (Spaces + CDN):
- Build locally or via CI, then upload the contents of `dist/` to a DigitalOcean Space and enable CDN.

Notes
- If you prefer automatic deployments, configure the App Platform to deploy on pushes to `main`.
- Update environment variables in DigitalOcean App settings if your app needs any.
# Welcome to your Lovable project

## Project info

**URL**: https://lovable.dev/projects/cfef9c18-a0de-4b65-b60e-63bccce96ff2

## How can I edit this code?

There are several ways of editing your application.

**Use Lovable**

Simply visit the [Lovable Project](https://lovable.dev/projects/cfef9c18-a0de-4b65-b60e-63bccce96ff2) and start prompting.

Changes made via Lovable will be committed automatically to this repo.

**Use your preferred IDE**

If you want to work locally using your own IDE, you can clone this repo and push changes. Pushed changes will also be reflected in Lovable.

The only requirement is having Node.js & npm installed - [install with nvm](https://github.com/nvm-sh/nvm#installing-and-updating)

Follow these steps:

```sh
# Step 1: Clone the repository using the project's Git URL.
git clone <YOUR_GIT_URL>

# Step 2: Navigate to the project directory.
cd <YOUR_PROJECT_NAME>

# Step 3: Install the necessary dependencies.
npm i

# Step 4: Start the development server with auto-reloading and an instant preview.
npm run dev
```

**Edit a file directly in GitHub**

- Navigate to the desired file(s).
- Click the "Edit" button (pencil icon) at the top right of the file view.
- Make your changes and commit the changes.

**Use GitHub Codespaces**

- Navigate to the main page of your repository.
- Click on the "Code" button (green button) near the top right.
- Select the "Codespaces" tab.
- Click on "New codespace" to launch a new Codespace environment.
- Edit files directly within the Codespace and commit and push your changes once you're done.

## What technologies are used for this project?

This project is built with:

- Vite
- TypeScript
- React
- shadcn-ui
- Tailwind CSS

## How can I deploy this project?

Simply open [Lovable](https://lovable.dev/projects/cfef9c18-a0de-4b65-b60e-63bccce96ff2) and click on Share -> Publish.

## Can I connect a custom domain to my Lovable project?

Yes, you can!

To connect a domain, navigate to Project > Settings > Domains and click Connect Domain.

Read more here: [Setting up a custom domain](https://docs.lovable.dev/features/custom-domain#custom-domain)
