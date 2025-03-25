# 📘 Project Handbook

## 🗂 Table of Contents
1. [Task Estimation in SCRUM](#task-estimation-in-scrum)
2. [Code Reviews](#code-reviews)
3. [Pull Requests](#pull-requests)
4. [Resources](#resources)

## 📋 Task Estimation in SCRUM

## 🧑‍💻 Code Reviews

## 🔄 Pull Requests
Pull Requests (PRs) are not just a technical formality. They are are a conversation between developers of the project and a safeguard for quality and an essential tool in modern software development.
Here are some best practices for Pull Requests:

---

### **1. Create Small Pull Requests**
> "Small is reviewable, and reviewable is mergeable." - Jason Lengstorf

**Why it matters:**

Large PRs are hard to read, meaning that reviewers will have a hard time understanding the changes. This can lead to a longer review time and more bugs slipping through the cracks.
Small PRs on the other hand:
- Are quicker to review and merge
- Have fewer conflicts
- Make changes easier to understand in and out of context
- Are easier to test

**📌 Tips:**

- Aim for PRs that include one feature, fix or refactor
- If the feature is too large, break it down into multiple PRs that can be reviewed independently

---

### **2. Write Useful Descriptions and Titles**
A good PR title and description can give context, explain intent and help reviewers know what to look for.

**Use a consistent commit/PR message convention**

Example:
`
feat(login): add password reset functionality
`

Here's what this message tells us:
- `feat`: This is a new feature
- `(login)`: This feature is related to the login functionality
- `add password reset functionality`: A brief description of the change

**Good PR description should include:**
- A summary of what was done
- A link to the relevant issue (if applicable)
- The why behind the change
- Any relavant decisions made

**📌 Tips:**

If a template is available, use it. If not, consider creating one for your team in `.github/PULL_REQUEST_TEMPLATE.md` to standardize PR descriptions.

---

### **3. Comment the Code and/or the PR**

Help yout reviewer help you.
Inline comments or PR-level notes can direct the reviewer's attention to specific parts of the code or non-ovious logic.
This reduces back-and-forth and speeds up the review process.

**Examples of when to comment:**
- When you're using an unfamiliar or non-standard pattern or library
- When something might be temporary or experimental
- When you're unsure about a decision and want feedback

---

### **4. Make it visual**

Show don't tell.
Reviewers often lack the full project context, esxpacially for UI/UX changes. Help them visualise your work when possible.

**Include:**
- **Screenshots** of UI changes
- **Screen recordings** of animations or complex flows
- **GIFs** showing before/after behavior

---

### **Final Tip: Respect the Review Process**

> "Don't just aim to get it merged. Aim to make it understandable, maintainable and respectful of your team's time." - Kent C. Dodds (adapted from Atlassian's Guide)

---

### **Sources & References:**
- [Altassian Blog: The Written Unwritten Guide to Pull Requests](https://www.atlassian.com/blog/git/written-unwritten-guide-pull-requests)
- [GitHub Docs: About Pull Requests](https://docs.github.com/en/pull-requests)
- [SmartBear: Best Practices for Peer Code Review](https://smartbear.com/learn/code-review/best-practices-for-peer-code-review/)
- Real-world dev experience

### 📊 Pull Request Workflow Diagram

Here's a simple flowchart to visualize the Pull Request workflow:

```mermaid
flowchart TD
    A[Create Feature Branch] --> B[Make & Test Changes]
    B --> C[Push to Remote Branch]
    C --> D[Open Pull Request]
    D --> E[Write Clear Title & Description]
    E --> F[Add Screenshots or Context (if needed)]
    F --> G[Submit for Review]
```

## 📚 Resources