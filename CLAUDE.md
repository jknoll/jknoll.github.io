# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This is a GitHub Pages personal website repository (`jknoll.github.com`) showcasing AI/ML projects, hackathon wins, professional skills, and certifications. The site is served directly from markdown files without Jekyll configuration.

## Content Structure

The repository contains:
- `index.md` - Main project page (original version)
- `index-new.md` - Enhanced version with skills and certifications sections
- `linkedin-skills.md` - Source data for professional skills (grouped by category)
- `linkedin-licenses-certifications.md` - Source data for certifications and credentials

## Dependency Management

This project uses Jekyll (Ruby) for site generation. Dependencies are managed with Bundler:
- Add Ruby gem dependencies to `Gemfile`
- Run `bundle install` to install dependencies
- Run `bundle update` to update dependencies 

## Content Management Approach

**When updating the main page:**
1. Skills and certifications should be sourced from the respective `.md` files in the root directory
2. The design pattern follows academicpages.github.io structure (sidebar + main content)
3. Sections without provided data should be commented out using HTML comments
4. Profile photos should use placeholder references until actual images are provided

**Content organization:**
- Introduction and project descriptions are the primary content
- Skills are grouped into logical categories (AI & ML, AI Agents & Orchestration, Engineering & Systems, Web3 & Product)
- Certifications are grouped by domain (AI & LLM Development, Product & Process)
- Each certification includes: issuing authority, issue date, skills, description, and credential link

## GitHub Pages Deployment

This repository uses Jekyll with GitHub Pages. Changes pushed to the `main` branch are automatically built by Jekyll and deployed to `https://jknoll.github.io`.

## Local Preview

To preview the Jekyll site locally before pushing:

**Using Jekyll (recommended):**
```bash
# Install dependencies (first time only)
bundle install

# Start Jekyll server
bundle exec jekyll serve

# Site will be available at http://localhost:4000
```

**Note:** Jekyll renders the site exactly as GitHub Pages will, including YAML front matter, layouts, and themes.

## Testing Changes

When modifying content:
1. Generate a new version as `index-new.md` first (per README.md instructions)
2. Test locally using Jekyll: `bundle exec jekyll serve`
3. Review visually at `http://localhost:4000` before replacing `index.md`

Do not proceed to step 4 without user review and approval:
4. Commit and push to deploy

## Testing Changes with Claude for Chrome

Claude Code integrates with the Claude in Chrome browser extension to enable autonomous visual QA and testing.

**Prerequisites:**
- Google Chrome browser
- Claude in Chrome extension (v1.0.36+) from [Chrome Web Store](https://chromewebstore.google.com/detail/claude/fcoeoabgfenejglbffodgkkbkcdhcgfn)
- Claude Code CLI (v2.0.73+)
- Paid Claude plan (Pro, Team, or Enterprise)

**Enable Chrome integration:**

Chrome integration must be enabled at launch time with the `--chrome` flag:
```bash
claude --chrome
```

Note: The `/chrome` command in an existing session only allows enabling by default (which applies to all future sessions). To enable for a single session without affecting future sessions, you must launch with `--chrome`.

**Workflow for visual QA:**
1. Start Jekyll server: `bundle exec jekyll serve`
2. Launch Claude Code with Chrome enabled: `claude --chrome` (or relaunch if already running)
3. Ask Claude to navigate to `http://localhost:4000`
4. Claude will:
   - Open the page in Chrome
   - Visually inspect the rendered markdown
   - Test interactions and layout
   - Read console logs if needed
   - Provide detailed QA feedback
   - Iterate on fixes until page looks correct

**Available capabilities:**
- Navigate pages and click elements
- Read page content and visual rendering
- Check console logs and network requests
- Scroll and interact with the page
- Verify design implementation
- Test responsive behavior

See [official docs](https://code.claude.com/docs/en/chrome) for full details.

## Git Workflow

Standard workflow:
```bash
git add .
git commit -m "Description of changes"
git push origin main
```

The remote is: `git@github.com:jknoll/jknoll.github.com.git`
