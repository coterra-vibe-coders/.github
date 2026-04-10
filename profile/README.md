# 🚀 Welcome to the Coterra VibeCode Crew

You're here because you have ideas that could make Coterra better — and now you have the tools to build them.

VibeCode Crew is a community of builders across Coterra who are turning ideas into working applications using AI-assisted development. No CS degree required. No ticketing system. Just you, a problem worth solving, and an AI coding partner.
What This Is

A structured path from idea to working app. You'll get access to pre-configured development environments, AI coding tools, and a community of people doing the same thing. Build tools for your team, automate a workflow that's been bugging you, or prototype something nobody's thought of yet.

# GitHub Copilot Onboarding Guide for Vibecoders

## Prerequisites

*   A Coterra-managed GitHub Copilot license (you'll receive an invite)
    
*   A GitHub account (personal or new — covered below)
    
*   VS Code installed locally (version **1.96 or later** recommended)
    

* * *

## Step 1: Accept Your GitHub Copilot Invite

1.  Check your email (the address your admin has on file) for an invite from **GitHub** to join the Copilot organization.
    
2.  Click the **"Accept invitation"** link in the email.
    
3.  If you don't see the email, check your spam/junk folder. If it's still missing, reach out to whoever manages your Copilot licenses.
    

* * *

## Step 2: Create or Link Your GitHub Account

### If you already have a GitHub account:

1.  Go to [github.com](https://github.com) and sign in.
    
2.  Make sure the invite from Step 1 was sent to the email associated with this account. If not, go to **Settings → Emails** and add the email address that received the invite, then accept the invite again.
    

### If you need to create an account:

1.  Go to [github.com/signup](https://github.com/signup).
    
2.  Use the email address that received the Copilot invite.
    
3.  Follow the prompts to set a username and password.
    
4.  Verify your email when prompted.
    
5.  Return to the invite email and accept it.
    

* * *

## Step 3: Download & Install VS Code

> Skip this if you already have VS Code installed. Make sure you're on **version 1.96 or later** (`Help → About` to check).

1.  Go to [code.visualstudio.com](https://code.visualstudio.com).
    
2.  Download the installer for your OS (Windows/Mac/Linux).
    
3.  Run the installer with default settings.
    
    *   **Windows tip:** Check the boxes for _"Add to PATH"_ and _"Add 'Open with Code' to context menu"_ — both are useful.
        
4.  Launch VS Code after installation.
    

* * *

## Step 4: Sign In to GitHub Copilot

> **Note:** In recent versions of VS Code, Copilot is built in. You do **not** need to sign in via the Accounts icon. Instead, use the **Copilot icon in the bottom-right Status Bar**.

1.  Open VS Code.
    
2.  Look at the **bottom-right corner** of the window. You should see a **Copilot icon** (sparkle/chat icon) in the Status Bar.
    
3.  **Hover over** the Copilot icon and click **"Use AI Features"** (or click the icon directly if prompted to sign in).
    
4.  When prompted, choose **"Sign in with GitHub"** and follow the browser prompts to authenticate with the GitHub account you used to accept the invite.
    
5.  Allow the browser to redirect back to VS Code when prompted.
    

> **Important:** If VS Code instead prompts you to "Sign in to GHE.com," you do **not** need to do that — choose the standard **GitHub.com** sign-in option. The Coterra Copilot license is managed through a GitHub.com organization, not a GHE.com instance. If you're stuck on the GHE prompt, see the Troubleshooting section below.

* * *

## Step 5: Verify Copilot Is Working

1.  After signing in, **click the Copilot icon** in the bottom-right Status Bar.
    
2.  A status dashboard should appear. Confirm it shows **"Copilot Enterprise Usage"** at the top — this means your Coterra organization license is active.
    
    *   You should see **Inline Suggestions: Included**, **Chat messages: Included**, and a **premium requests** usage bar.
        
3.  To test inline suggestions: open or create any code file (e.g., a `.py` or `.js` file), type a comment like `# function to calculate the sum of a list`, and press **Enter**. You should see gray **ghost text** suggestions. Press **Tab** to accept.
    
4.  To test Copilot Chat: open the Chat panel via the sidebar chat icon (or `Ctrl+Shift+I` / `Cmd+Shift+I`) and ask a question.
    

* * *

## Step 6: Install the GitHub Copilot Extension (If Needed)

> In **VS Code 1.96+**, Copilot is built in and the extension installs automatically when you sign in. Only follow these steps if you don't see the Copilot icon in the Status Bar after signing in.

1.  In VS Code, open the **Extensions** panel (`Ctrl+Shift+X` / `Cmd+Shift+X`).
    
2.  Search for **"GitHub Copilot"**.
    
3.  Install **GitHub Copilot** (published by GitHub). This will also install **GitHub Copilot Chat** as a dependency.
    
4.  After installation, you may see a notification asking you to sign in — follow the prompts if so, then return to Step 4.
    

* * *

## Troubleshooting

| Issue | Fix |
| --- | --- |
| **No invite email** | Check spam; confirm your admin has the correct email; ask them to resend. |
| **"You don't have access to Copilot"** | Your invite may not be accepted, or there's an email/account mismatch — revisit Steps 1–2. |
| **No Copilot icon in the Status Bar** | Make sure you're on VS Code 1.96+. If the icon was moved, click the `{ }` language status icon in the bottom-right bar — Copilot may be nested there. You can pin it back to the Status Bar from that menu. |
| **Stuck on "Sign in to GHE.com" / forced to use GitHub Enterprise auth** | Open the Command Palette (`Ctrl+Shift+P` / `Cmd+Shift+P`) → **"Preferences: Open User Settings (JSON)"**. If you see `"github.copilot.advanced": { "authProvider": "github-enterprise" }`, **delete that entire block**, save, and restart VS Code. This resets Copilot to use standard GitHub.com auth. |
| **Status dashboard does NOT say "Copilot Enterprise Usage"** | You may be signed into the wrong GitHub account, or the org license isn't linked. Go to the **Accounts** icon (bottom-left sidebar) → sign out → sign back in using the Copilot Status Bar icon, making sure to use the GitHub account that received the invite. |
| **Extension installed but no suggestions** | Click the Copilot icon in the Status Bar to check the dashboard. Confirm "Inline Suggestions" shows checkmarks for **All files** and your language. If Copilot shows as disabled, click to re-enable. |
| **Browser auth redirect fails** | Try the auth flow again. If on VPN, try temporarily disconnecting. |
| **Firewall/proxy blocks Copilot** | Copilot needs access to `*.github.com` and `*.githubcopilot.com` — check with IT if these are blocked. |
