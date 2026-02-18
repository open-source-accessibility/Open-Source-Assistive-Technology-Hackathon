# GitHub Learning Room

During the Open Source Assistive Technology Hackathon, we’ll walk through core GitHub contribution workflows (including NVDA and keyboard-only navigation), so participants can practice navigating repositories, issues, pull requests, and code reviews with confidence. Whether you’re new to contributing or ready to level up, you’ll leave with practical experience and a clear path to ongoing open source involvement.

## Goals

### 1) Build confidence navigating GitHub workflows (NVDA and keyboard-only)

### 2) Teach the end-to-end “contribute to an open source repo” flow

### 3) Provide multiple “on-ramps” so everyone can contribute meaningfully

---

## Day 1: Intro

### GitHub Orientation (what things are and where to find them)
#### Steps
1. Explain core GitHub building blocks:
   - Repository, organization, maintainer, contributor
2. Show the difference between:
   - Issues (work items/bugs/requests)
   - Pull Requests (proposed changes)
   - Discussions (Q&A and community conversation)
3. Explain branching at a practical level:
   - Default branch vs feature branch
   - Why branches exist (safe collaboration + review)
4. Introduce coordination tools (what they are / when they matter):
   - Releases and tags (shipping versions)
   - Projects (boards for planning)
   - Milestones (grouping work by time/version)

### Settings (recommended browser + NVDA setup)
#### Steps
1. Confirm the recommended browser for the event (and version).
2. Configure NVDA basics for web work (for those using NVDA):
   - Practice toggling browse/focus mode on form-heavy pages
3. Review GitHub preferences and accessibility-related settings (as applicable):
   - Notification settings (avoid missing review requests)
   - Email visibility / security preferences (participant comfort + safety)
   - [Accessibility settings](https://docs.github.com/en/account-and-profile/how-tos/account-settings/managing-accessibility-settings)
4. Do a quick “sanity check” flow:
    1. Confirm everyone can sign into GitHub and reach their profile page.
    2. Review essential keyboard concepts:
        - Tab / Shift+Tab, Enter, Space, Escape
        - Browser find (Ctrl+F), address bar focus, back/forward navigation
    3. Review essential NVDA concepts:
        - Browse mode vs focus mode (when to switch)
        - Heading navigation, landmarks, links list, form fields navigation
    4. Practice reading and understanding page structure on GitHub pages (note different pages have different setups):
        - Identify page title, primary navigation, and main content region.
    5. Validate participants can reliably:
        - Navigate to a repository
        - Open an issue list
        - Open a pull request list
        - Return to previous pages without losing context

### Screen reader / keyboard navigation (hands-on page navigation drills)
#### Steps
1. Repositories page drill:
   - Open a repository
   - Find README, file list, and key tabs (Code, Issues, Pull requests)
   - Use headings/landmarks to move between sections
   - Resource: https://accessibility.github.com/documentation/guide/repos/
2. Issues page drill:
   - Open Issues tab
   - Filter issues (label, is:open, author, etc.)
   - Open an issue, read description, scan comments, add a comment
   - Resource: https://accessibility.github.com/documentation/guide/issues/
3. Pull Requests page drill:
   - Open Pull requests tab
   - Filter PRs (is:open, review-requested, author, etc.)
   - Open a PR, locate description, commits/files changed, checks/status
   - Resource: https://accessibility.github.com/documentation/guide/pull-requests/
4. Code review drill:
   - Open “Files changed”
   - Move through diffs and locate review comment controls
   - Add a single comment and submit a review (comment-only)
   - Practice returning to conversation tab and finding reviewer feedback

### Best Practices (what “good participation” looks like)
#### Steps
1. Explain “small PRs” and iterative review:
   - Keep changes focused
   - Expect back-and-forth
   - Be explicit about what you did and how you tested
2. Explain reverts at a high level:
   - Sometimes merged changes must be undone
   - Reverts are normal and not a failure
3. Teach how to write a strong accessibility issue report:
   - Expected vs actual behavior
   - Steps to reproduce
   - URL or repo/branch/commit
   - OS + version, browser + version
   - Assistive tech + version (e.g., NVDA version)
   - Device details (if relevant)
   - Provide a short recording or screenshots when possible
4. Teach basic labeling and workflow concepts:
   - What labels mean and how they’re used for prioritization
   - Don’t “spam” maintainers; ask clear questions and provide context
5. Teach community norms:
   - Read and follow the Code of Conduct
   - Use inclusive, respectful language
   - Be cautious when commenting on long-closed issues (provide new info, don’t +1)

---

## Day 2

### Copilot (how to use GitHub Copilot responsibly in contributions)
#### Steps
1. Explain what Copilot is and when it helps:
   - Drafting small code changes, tests, documentation
2. Explain constraints:
   - Always review generated code for correctness and security
   - Ensure licensing and project contribution rules are followed
3. Show practical workflows:
   - Use Copilot to propose a small refactor
   - Use Copilot to generate test scaffolding
   - Use Copilot to draft a clear PR description
4. Accessibility note:
   - Validate generated UI code for keyboard and screen reader behavior

### Hands-on Activity (end-to-end contribution practice)
#### Steps
1. Find work:
   - Locate a repo’s Issues page
   - Filter issues by label (e.g., `good first issue`, `help wanted`)
   - Open an issue and read requirements and acceptance criteria
2. Collaborate:
   - Ask clarifying questions in an issue comment
   - Confirm maintainers’ preferred workflow (branching, testing, style)
   - Declare intent (“I’d like to take this”) and confirm assignment if needed
3. Make changes:
   - Fork (if needed) or create a feature branch
   - Edit files, run checks/tests, and commit changes
4. Open a PR:
   - Push branch and create a pull request
   - Fill in PR template, link the issue, describe changes, add testing notes
5. Respond to review:
   - Read review comments, ask follow-up questions, push updates
   - Re-request review when ready
6. Merge:
   - Confirm checks pass, handle merge conflicts if any
   - Merge using the repo’s preferred method (merge commit / squash / rebase)
   - Delete branch and verify the issue is closed (if applicable)

#### Steps (Alternative)
1. Documentation on-ramp:
   - Find docs pages that are unclear or outdated
   - Make a small improvement (typo fix, clarity, add example)
2. Triage on-ramp:
   - Reproduce an issue (if possible)
   - Add missing environment details and clearer reproduction steps
   - Suggest labels or confirm duplicates
3. Testing on-ramp:
   - Run the project locally (if feasible)
   - Validate a fix branch from someone else (or a draft PR)
   - Report results clearly (pass/fail + environment)
4. Small code change on-ramp:
   - Pick a contained task (copy tweak, error message, small UI fix)
   - Add/update tests if the project expects them
5. Accessibility-focused on-ramp:
   - Identify a keyboard trap, missing label, focus issue, or contrast issue
   - Document expected vs actual behavior with clear steps

### Activity Options
1. Add an issue template to a repository:
   - Create or update `.github/ISSUE_TEMPLATE/`
   - Include provided template (todo)
2. Log an accessibility issue:
   - Use the new template
   - Include a clear title and minimal reproduction steps
3. Update documentation:
   - Improve a README section or contributing guide
   - Add a “How to test with NVDA” section (if relevant)

### VS Code version (Copilot + accessible workflow)
#### Steps
1. Install VS Code and required extensions:
   - GitHub Copilot (and sign in)
2. Configure basic accessibility settings as needed:
   - Verify screen reader mode behavior
   - Confirm keyboard shortcuts for source control and diff navigation
3. Practice the “edit → commit → push → PR” loop from VS Code
4. Resource: https://accessibility.github.com/documentation/guide/github-copilot-vsc/


## Todos

- [ ] Create "easy to fix" starter repos/issues (for practice):
   - Create a small repo with intentional docs gaps or simple bugs
   - Add labels like `good first issue` and clear acceptance criteria
   - Ensure tasks can be completed within hackathon time
- [ ] Create `.github/ISSUE_TEMPLATE/` - @mlama007
