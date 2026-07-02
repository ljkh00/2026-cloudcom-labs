# ☁️ CloudEats Academy — Introduction to Cloud Computing

> **A 10-week, hands-on cloud computing course built around one real app.**
> Every concept is applied to *CloudEats* — a food delivery platform you build from a single Docker container all the way to a fully monitored, secured, and deployed system.

🌐 **Live course site:** [ljkh00.github.io/2026-cloudcom-labs](https://ljkh00.github.io/2026-cloudcom-labs)

---

## 📖 What this course is

This is a Diploma-level introduction to cloud computing. It assumes no prior cloud experience — just a willingness to follow steps, break things, and learn from what happens.

By the end of Week 10 you will have:

- Containerised a multi-service application with Docker and Docker Compose
- Set up relational and NoSQL databases in the cloud
- Split a monolith into microservices
- Built a CI/CD pipeline with GitHub Actions that tests and deploys on every push
- Secured an API with JWT authentication and role-based access control
- Monitored a live system with centralised logging and Prometheus metrics
- Written a cloud migration plan for a real production scenario

---

## 🎯 Who this is for

| Track | Who | What to expect |
|---|---|---|
| 🌱 **Beginner** | First time using a terminal or Docker | Every step expanded, plain-English definitions, inline troubleshooting |
| ⚡ **Average** | Comfortable with a terminal, some coding experience | Collapsed steps, "why are we doing this?" callouts, checkpoint questions |
| 🚀 **Advanced** | Docker and Linux experience | Challenge extensions, trade-off discussions, production-grade context |

Every lecture and lab supports all three tracks. Switch between them at any time using the pace selector at the top of each page — no separate courses, no separate files.

---

## 🗂️ Course structure

| Week | Topic | Labs |
|---|---|---|
| 01 | Foundations of Cloud Computing | Dev environment setup |
| 02 | Core Cloud Services | Static menu container · Docker networking |
| 03 | Databases in the Cloud | Docker Compose + MySQL · User registration |
| 04 | Cloud-Native Applications | Relational queries · Redis + MongoDB |
| 05 | Microservices Architecture | Service decomposition · API Gateway (advanced) |
| 06 | DevOps & Version Control | Git branching · Automated testing (CI) |
| 07 | CI/CD & Infrastructure as Code | Infrastructure as Code · Deployment automation (CD) |
| 08 | Cloud Security & Access Control | JWT authentication · RBAC access control |
| 09 | Monitoring, Logging & Optimisation | Application logging · Performance monitoring |
| 10 | Emerging Trends & Course Wrap-up | Cloud migration plan |

---

## 🚀 How to use this course

### Option A — Use the live site (recommended)
Visit the GitHub Pages link above. No setup required. Works on any device.

### Option B — Run locally
```bash
git clone https://github.com/ljkh00/2026-cloudcom-labs.git
cd 2026-cloudcom-labs
# Open index.html in your browser — no build step needed
open index.html        # macOS
xdg-open index.html    # Linux
start index.html       # Windows
```

### What you need before Week 1
- A computer that can run a virtual machine (8 GB RAM recommended)
- No cloud account required — all labs run locally using Docker and Proxmox
- Full setup instructions are in [Lab 1.1 — Dev Environment](week01/lab1_dev_environment.html)

---

## 🏗️ Repository structure

```
/
├── index.html                  ← Course landing page
├── .nojekyll                   ← GitHub Pages config
├── lab_index.md                ← File inventory and maintenance reference
├── week01/
│   ├── index.html              ← Lecture
│   └── lab1_dev_environment.html
├── week02/
│   ├── index.html
│   ├── lab1_static_menu.html
│   └── lab2_docker_networking.html
│   ...                         ← weeks 03–09 follow the same pattern
└── week10/
    ├── index.html
    └── lab1_cloud_migration_plan.html
```

Each week folder contains one lecture file (`index.html`) and one or two lab files.

---

## 🛠️ Built with

- Plain HTML, CSS, JavaScript — no framework, no build step, no dependencies
- Runs entirely in the browser
- Hosted on GitHub Pages
- Designed mobile-first for students accessing from phones

---

## 📄 Licence

Course content © 2026 CloudEats Academy. All rights reserved.

Sharing links to the live site is encouraged. Reproducing or republishing the content without permission is not.

---

## 🤝 Contributing

This course is currently maintained by a single instructor. If you spot a broken step, outdated command, or unclear explanation, please open an issue and describe what went wrong and what you expected to happen.

Pull requests for typo fixes and broken links are welcome.
