# 🧠 Odin Project Git & VS Code Setup Guide

A personal quick reference for cloning, pushing, and managing Odin Project repositories with GitHub and VS Code.

---

## 🚀 1. Starting a New Odin Project

1. Go to the lesson page and open the **GitHub starter repo** link.
2. Click **Fork** → this makes your own copy under `https://github.com/todduxer/...`
3. Click the green **Code** button → copy the **HTTPS** URL.

Example:


4. In VS Code’s terminal:
```bash
cd ~/Projects
git clone https://github.com/todduxer/odin-links-and-images.git
cd odin-links-and-images
code .


Absolutely 💪 — that’s a *perfect* habit to build early, Todd.
You can (and should) keep this documented directly inside your VS Code workspace — as a `README.md` file.

Here’s exactly how to do it and a template you can reuse 👇

---

## 🪄 **How to keep your personal setup notes inside VS Code**

### 🗂 Step 1: Create a README file

In VS Code:

1. Open the folder where you want your notes (for example your `~/Projects` folder or inside your Odin project).
2. In the Explorer sidebar, click **New File ➕**
3. Name it:

   ```
   README.md
   ```

VS Code automatically gives `.md` files (Markdown) rich formatting — headings, lists, code blocks, etc.

---

### 🧾 Step 2: Paste this starter README template

```markdown
# 🧠 Odin Project Git & VS Code Setup Guide

A personal quick reference for cloning, pushing, and managing Odin Project repositories with GitHub and VS Code.

---

## 🚀 1. Starting a New Odin Project

1. Go to the lesson page and open the **GitHub starter repo** link.
2. Click **Fork** → this makes your own copy under `https://github.com/todduxer/...`
3. Click the green **Code** button → copy the **HTTPS** URL.

Example:
```

[https://github.com/todduxer/odin-links-and-images.git](https://github.com/todduxer/odin-links-and-images.git)

````

4. In VS Code’s terminal:
```bash
cd ~/Projects
git clone https://github.com/todduxer/odin-links-and-images.git
cd odin-links-and-images
code .
````

---

## 💻 2. Making Changes & Committing

When you’ve added or edited files:

```bash
git add .
git commit -m "Describe what you changed"
git push
```

💡 **Tip:** Use meaningful messages like
`Add homepage link and dog image to index.html`

---

## 🔗 3. Linking Local Repo to GitHub

If you ever need to manually connect:

```bash
git remote add origin https://github.com/todduxer/your-repo-name.git
git branch -M main
git push -u origin main
```

Verify with:

```bash
git remote -v
```

---

## 🧩 4. Common Git Commands

| Action                  | Command                        |
| ----------------------- | ------------------------------ |
| Check repo status       | `git status`                   |
| See recent commits      | `git log --oneline`            |
| Create new branch       | `git checkout -b feature-name` |
| Switch branches         | `git checkout main`            |
| Pull latest from GitHub | `git pull`                     |

---

## 🧱 5. GitHub CLI Quick Reference

Authenticate once:

```bash
gh auth login
```

Check login status:

```bash
gh auth status
```

Create a new GitHub repo from VS Code:

```bash
gh repo create
```

---

## 🧠 6. My Personal Notes

* ✅ Always fork the original Odin repo first.
* ✅ Use `main` (not `master`) for new projects.
* ✅ Commit small, meaningful chunks often.
* ✅ Always push before closing VS Code for the day.

---

*Last updated:* `$(date +"%B %d, %Y")`

```

---

### 🧩 Step 3: Keep it visible in VS Code
You can:
- Pin the README tab (right-click → **Pin**) so it stays open.  
- Or, open it side-by-side with your code (drag to the right).  
- You can also keep all Odin notes in a dedicated folder like:
```

~/Projects/OdinNotes/README.md

```

---

### ✨ Bonus Tip: Turn it into a reusable “template”
Create one global copy of this file — e.g.,
```

~/Projects/Odin-Setup-Guide/README.md

````
Then every time you start a new Odin project, copy it in:
```bash
cp ~/Projects/Odin-Setup-Guide/README.md ~/Projects/odin-links-and-images/
````

---

Would you like me to format that README so it uses your actual GitHub username and project folder path automatically (so it’s “ready to copy-paste” for your setup)?
