# README

Version: 0.1

## Emergent Software AI-Ready Brand Kit

Think of it as `package.json` for our brand. One place where AI tools go to get a persistent, structured understanding of our visual identity. Instead of hoping the agent guesses our brand correctly, we just hand it a structured playbook. Colors, fonts, logos, components, writing style, the whole stack.

## Table of Contents

<ol>
  <li><a href="#claude">Claude</a></li>
  <li><a href="#copilot">Copilot</a></li>
</ol>

## Working with Claude

### Chat

> **Note** Claude's chat is not able to render images from SharePoint, this includes our logo. You can download the images needed from SharePoint then attach them directly to your chat.

1. Start a new chat in Claude
2. Connect Microsoft 365 if it isn't already connected by asking Claude to `Connect to SharePoint` and follow the authentication prompt that appears
3. Confirm Claude can see the brand kit by asking it to search for the folder `Search SharePoint for the Emergent Software AI-Ready Brand Kit folder`
4. Have Claude load the core brand files by asking it to `read brand-kit.md, design.md, logo-usage.md, font-usage.md, icon-usage.md, voice.md, and boilerplate.md from the folder`
5. Paste in the standardized starter prompt found at the end of `brand-kit.md`, making sure to add a high level description for your specific task in the `### Task` section
6. Run an initial test, such as asking for a simple webpage section, a button component, or a one-slide presentation layout, then confirm Claude applies the correct colors, fonts, and logo file
7. If anything looks off-brand, point Claude to the specific rule it missed (e.g. "check logo-usage.md — you used the wrong logo for a dark background") so it can correct course
8. Once verified, this same chat can continue to be used for the rest of that work session, since Claude retains the brand context for the whole conversation

### Claude Code

1. Install Claude Code via the terminal: `npm install -g @anthropic-ai/claude-code`
2. Authenticate by running `claude` in your terminal and following the login prompt
3. Navigate to your project's root directory before starting any brand-related work so Claude Code has the right file context
4. Connect Microsoft 365 by running `/mcp` in the Claude Code session and adding the Microsoft 365 MCP server so Claude Code can access SharePoint assets directly
5. Create a `CLAUDE.md` file in your project root and paste in our base prompt. Add any project-specific context below it (tech stack, framework, component library, file structure conventions)
6. Add the SharePoint brand kit path to `CLAUDE.md` so Claude Code knows where to pull assets: `Documents > Identity > Emergent Software AI-Ready Brand Kit`
7. Run an initial test by asking Claude Code to generate a branded component in your framework of choice, e.g. a primary button or a hero section, and verify it uses the correct colors, fonts, and logo
8. Check that generated CSS uses `var(--token-name)` rather than hardcoded hex values — if raw hex appears, remind Claude Code to reference the token system from `design.md`
9. For icon usage, confirm Claude Code is pulling from the `icons/` folder in the brand kit rather than importing a third-party icon library that may conflict with the Solid icon style rule
10. Add a `.claudeignore` file if needed to prevent Claude Code from scanning large asset folders like fonts or raw photography that aren't relevant to code generation
11. Commit `CLAUDE.md` to your repo so every developer on the team gets the same brand context automatically when they run Claude Code in the project

> **Tip** Claude Code works best when our design tokens are defined locally in a `tokens.css` or `variables.css` file in the project. Ask Claude Code to generate this file from `design.md` on first setup so the tokens exist in the codebase and Claude doesn't have to rely solely on our brand kit documentation

## Working with Copilot

### M365 Chat

> Not available
