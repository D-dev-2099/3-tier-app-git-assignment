# 3-tier-app-git-assignment
## 🔁 Branching Strategy

- main → For stable, production-ready code
- dev → Where all teams test their code together
- feature/frontend-login → For frontend development
- feature/backend-auth → For backend API
- feature/infra-vpc → For infrastructure setup (Terraform)

Merge flow:  
feature branches → dev → main
