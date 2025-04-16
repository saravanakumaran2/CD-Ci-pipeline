# CI/CD Pipeline with Jenkins

This is a simple project where I tried building a **CI/CD pipeline using Jenkins**. The goal was to automate the process of building, testing, and deploying a project — all in one flow.

---

##  What I Did in This Project

- Created a `Jenkinsfile` that defines my CI/CD stages
- Added test steps to simulate automated checks
- Used **Docker** to containerize the app (or plan to in future)
- Set up a deploy step (can be to Docker or remote server)
- Practiced full automation from GitHub to deployment

---

## Pipeline Flow (as in the Jenkinsfile)

1. **Pull Code** – Jenkins checks out code from GitHub
2. **Build** – Could be Docker build or app build step
3. **Test** – Runs test scripts or commands (mocked in this version)
4. **Deploy** – Sends build to a server or environment (can be local or cloud)

---

## What’s in the Repo

```bash
.
├── Jenkinsfile         
└── README.md           
```

---

##  Notes

- Make sure Jenkins is linked to GitHub using correct credentials
- Docker must be installed on Jenkins if using `docker build`
- You can expand this to:
  - Add Slack/email notifications
  - Use `post` blocks to show success/failure messages
  - Integrate SonarQube for code quality
- Add proper error handling in stages using `try/catch`

---


