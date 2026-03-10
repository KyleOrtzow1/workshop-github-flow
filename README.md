# GitHub Workflow Crash Course

**Branches, Pull Requests, and Review — in 90 minutes**

Learn the collaborative GitHub workflow used by teams everywhere: branch, commit, open a pull request, review a peer's work, and merge.

---

## Workshop Resources

| Resource | Link |
|----------|------|
| Slide Deck | [Google Slides](https://docs.google.com/presentation/d/1qLpQaARheXQJa6kKl11HGAspaPx5VDae/edit?usp=sharing&ouid=102856528565907542087&rtpof=true&sd=true) |
| Setup / Install Instructions | [Google Doc](https://docs.google.com/document/d/1oqwpv5qoaiLuTeQNCmqBXlsmR6acIyag4J-Qm_MkP64/edit?usp=sharing) |
| Git Commands Cheat Sheet | [Google Doc](https://docs.google.com/document/d/1lAIlFAb0uMlCjrsgZ4GhrrpA90-QWj5CLwbO68fxwlc/edit?usp=sharing) |

---

## What You'll Do

1. **Fork** this repo to your own GitHub account
2. **Clone** it (or open a Codespace)
3. **Create a branch** (e.g. `add-your-name`)
4. **Edit** `participants.md` — add your name, GitHub handle, and one goal
5. **Commit and push** your branch
6. **Open a Pull Request** using the provided template
7. **Review** a partner's PR using the "I Like / I Wish / What If" framework
8. **Update** your PR based on feedback and merge

---

## Getting Started

### Option A: GitHub Codespaces (recommended — no install needed)

1. Fork this repo (click **Fork** at the top right)
2. On your fork, click **Code** > **Create codespace on main**
3. You're ready — the editor opens in your browser

### Option B: Local Setup

1. Fork this repo
2. Clone your fork:
   ```bash
   git clone https://github.com/YOUR-USERNAME/workshop-github-flow.git
   cd workshop-github-flow
   ```
3. Open the project in your editor

> **Need help with Git installation?** See the [Setup Instructions](https://docs.google.com/document/d/1oqwpv5qoaiLuTeQNCmqBXlsmR6acIyag4J-Qm_MkP64/edit?usp=sharing).

---

## The Task

1. Create a new branch:
   ```bash
   git checkout -b add-your-name
   ```
2. Open `participants.md` and add a new row with your info
3. Commit your change:
   ```bash
   git add participants.md
   git commit -m "Add [your name] to participants"
   ```
4. Push your branch:
   ```bash
   git push origin add-your-name
   ```
5. Go to GitHub and open a **Pull Request** from your branch into `main`
   - Use the PR template — fill in every section

---

## Review Guide

When reviewing a partner's PR, use the **"I Like / I Wish / What If"** framework:

- **2 line comments:**
  - **I like...** — specific praise (clarity, naming, structure)
  - **I wish...** — specific improvement request
- **1 summary comment:**
  - **What if...** — a suggestion or alternative
- Choose **Approve** or **Request changes**

See [`examples/review.md`](examples/review.md) for a full walkthrough.

---

## Agenda (90 minutes)

| Time | Activity |
|------|----------|
| 0–5 min | Welcome + outcomes |
| 5–10 min | Hook: Pain / Dream / Fix |
| 10–20 min | Setup (Codespaces or local) |
| 20–30 min | Live demo: the full workflow |
| 30–55 min | Guided build: everyone makes a PR |
| 55–75 min | Peer review studio |
| 75–85 min | Apply feedback + update PR |
| 85–90 min | Wrap-up + resources |

---

## Troubleshooting

<details>
<summary><strong>"Authentication failed" when pushing</strong></summary>

- Make sure you're pushing to **your fork**, not the original repo
- If using HTTPS, you may need a [Personal Access Token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) instead of your password
- If using Codespaces, auth is handled automatically
</details>

<details>
<summary><strong>"I don't see the branch on GitHub"</strong></summary>

- Make sure you ran `git push origin your-branch-name`
- Check that you're looking at **your fork**, not the original repo
- On GitHub, click the branch dropdown to see all branches
</details>

<details>
<summary><strong>"Where is the Pull Request button?"</strong></summary>

- After pushing, GitHub often shows a yellow banner with **"Compare & pull request"** — click that
- Or go to the **Pull requests** tab and click **New pull request**
- Make sure the base is `main` and the compare branch is yours
</details>

<details>
<summary><strong>"I accidentally committed to main"</strong></summary>

- Don't panic! Create a new branch from where you are: `git checkout -b add-your-name`
- Your changes are now on the new branch
- Ask an instructor for help resetting main if needed
</details>

<details>
<summary><strong>"Merge conflict"</strong></summary>

- This can happen if someone else edited the same lines in `participants.md`
- Open the file, look for `<<<<<<<` markers, keep both entries, remove the markers
- Commit the fix and push again
</details>

---

## After the Workshop

- Keep this repo — it's yours to reference
- Check the [Git Commands Cheat Sheet](https://docs.google.com/document/d/1lAIlFAb0uMlCjrsgZ4GhrrpA90-QWj5CLwbO68fxwlc/edit?usp=sharing) whenever you need a refresher
- Practice by contributing to open source projects on GitHub
