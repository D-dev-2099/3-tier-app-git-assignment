# 3-tier-app-git-assignment
## 🔁 1.Branching Strategy

- main → For stable, production-ready code
- dev → Where all teams test their code together
- feature/frontend-login → For frontend development
- feature/backend-auth → For backend API
- feature/infra-vpc → For infrastructure setup (Terraform)

Merge flow:  
feature branches → dev → main

 2. What if someone pushes broken code directly to main?
This means your production site is now broken. What to do?

✍️ What to write:
markdown
Copy
Edit
## 💥 Handling Buggy Code in Main

1. Revert the commit using `git revert <commit-id>`
2. Create a hotfix branch to fix and test the issue
3. Merge the hotfix back to `main`
4. Add branch protection rules so no one can push directly to `main`
