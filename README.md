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
3. 3. How do you use Git Tags in a CI/CD pipeline?
Tags are like labels for versions. In DevOps, we use them to deploy specific versions of the code.

✍️ What to write:
markdown
Copy
Edit
## 🧪 Git Tags in CI/CD

- Tags like `v1.0` mark release versions
- CI/CD tools (like GitHub Actions, Jenkins) can auto-deploy when a tag is pushed
- Example: 
   - Developer runs `git tag -a v1.0 -m "Release v1.0"`
   - CI/CD picks this tag and deploys that version
