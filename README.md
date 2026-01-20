# 👨🏻‍💻 Conference Room Booking System

This repository contains a practice project used to demonstrate professional Git, GitHub, and collaboration workflows.  
The project simulates a **Conference Room Booking System** that will be expanded over multiple modules to support learning around documentation, APIs, teamwork, and system handover.

## 📌 Purpose of This Repository

This repository serves as a hands-on environment for:

- Practicing Git and GitHub fundamentals, including branching, committing, and merging.
- Creating and reviewing Pull Requests as a means of structured communication and code review.
- Working with sprint documentation to simulate real-world Agile processes.
- Gradually improving project documentation over time to support onboarding and maintainability.

At this stage, the repository emphasizes **process, communication, and foundational setup** rather than a fully implemented system. It is designed for trainees and developers to experiment with professional workflows in a low-stakes environment.

## 🗂 Repository Contents

- **README.md** – This comprehensive onboarding and overview document
- **docs/** – Key sprint documentation artefacts
  - `user-stories.md` – User stories and acceptance criteria
  - `epics.md` – Grouping of stories into logical epics (e.g., Employee Features, Admin Features)
  - `estimation.md` – Velocity calculation, team estimation, and story points
  - `priority-matrix.md` – Business value vs. effort/complexity prioritization
  - `sprint-1-review.md` – Sprint review summary with outcomes and lessons learned
- **LICENSE** – Project license (MIT)

As the project evolves, folders like `src/` (source code), `tests/` (unit tests), and `.github/` (workflows and issue templates) will be added.

## ⚙️ Installation

This project is in early stages and does not require full installation yet. However, for basic setup and to interact with documentation or future code:

### Prerequisites
- Git (version 2.25+ recommended)
- A GitHub account for forking/cloning and collaborating
- Optional: Node.js (v18+) or Python (v3.10+) if experimenting with prototype code in future iterations
- Text editor or IDE (e.g., VS Code) for viewing/editing markdown files

### Quick Setup
1. Clone the repository  
   ```bash
   git clone https://github.com/JuniorSillo/conference-room-booking-user-stories.git
   cd conference-room-booking-user-stories
   ```
2. (Future: Install dependencies if code is added, e.g., `npm install` or `pip install -r requirements.txt`.)
3. Explore the docs: Open files in `docs/` to review sprint artefacts.

No database or server setup is needed at this point, but placeholders for Docker or local dev environments will be added later.

## 🚀 Usage

This repository is currently used for:

1. Reviewing and evolving documentation practices to ensure clarity and accessibility.
2. Creating Pull Requests to propose changes, discuss improvements, and collaborate.
3. Simulating Scrum sprints through artefact creation and peer reviews.

**Example workflow**:
- Fork the repo for personal experiments.
- Create a branch for a new feature or doc update.
- Submit a PR and engage in reviews.

In future modules, usage will expand to running a web app for booking rooms, querying APIs, and testing features.

## 🤝 Contributing

We follow a collaborative, professional workflow to ensure high-quality contributions. Changes are **never** pushed directly to the `main` branch.

### Contribution Workflow (GitHub Flow)
1. Create a branch from `main`  
   ```bash
   git checkout -b feature/your-feature   # or docs/improve-something
   ```
2. Make changes and commit with conventional messages  
   e.g., `docs(readme): add onboarding section`, `feat: add new user story`
3. Push the branch  
   ```bash
   git push origin your-branch-name
   ```
4. Open a Pull Request on GitHub  
   - Descriptive title  
   - Body explaining **why** (purpose), **what** changed, and what to review  
   - Reference sprint artefacts or issues
5. Request reviews from at least one peer/teammate
6. Address feedback and iterate
7. Merge when approved (squash recommended for clean history)

Pull Requests are communication artefacts — use the description to document intent and decisions. For reporting issues or suggesting features, use GitHub Issues with templates (see `.github/ISSUE_TEMPLATE/`).

## Developer Onboarding (In Progress)

* This project is developed incrementally as part of a Software training program. The purpose of this section is to help new contributors to understand  
* What this system is intended to become  
* How documentation is organised  
* Where to find key project artefacts  
* What technologies will be used to develop this project?

### What this system is intended to become
The Conference Room Booking System will grow into a practical web application for managing meeting spaces. Employees will check availability, book/cancel rooms, and avoid conflicts. Admins will manage rooms and view reports.  
It solves real scheduling pain points while teaching clean code, APIs, and handover practices.

### System Context (High-Level)
- **Room Availability**: Track rooms, capacities, amenities.
- **Booking Requests**: Validate dates/times.
- **Conflict Prevention**: Prevent overlaps.
- **Administration Oversight**: Approvals, reports.
- **Future**: Calendar sync, notifications.

Components (planned):
- **Frontend**: React or HTML/JS UI
- **Backend**: Node.js/Express or Python/FastAPI
- **Database**: PostgreSQL/MongoDB
- **Auth**: JWT/sessions

Currently documented only via sprint artefacts.

### How documentation is organised
- **README.md**: Onboarding hub and overview
- **docs/**: All sprint artefacts (user stories, epics, etc.) — single source of truth

### Where to find key project artefacts
Read in this order:
1. `docs/user-stories.md` → Core requirements
2. `docs/epics.md` → Feature groupings
3. `docs/priority-matrix.md` → Prioritization
4. `docs/estimation.md` → Story points & velocity
5. `docs/sprint-1-review.md` → Outcomes & lessons

### Technologies used/planned
- **Now**: Git + GitHub, Markdown
- **Future**: JS/Node (or Python), SQL/NoSQL DB, Docker, Jest/Pytest

Start here: Read this README → browse `docs/` → make a small PR!

## Project Documentation

This repository contains sprint documentation from Scrum simulations:
- Files in `docs/` represent real sprint evolution — review them for decisions and progress.

## Upcoming Documentation
- API Documentation (Swagger/OpenAPI)
- Runtime Instructions (Docker Compose)
- Detailed Developer Setup
- Testing Guide
- Security & Best Practices

## LICENSE
This project is licensed under the MIT License — see the [LICENSE](LICENSE) file.

## ✍️ Author
Moeketsi Junior Sillo: sillojunior8@gmail.com  
Created as part of Software Development Trainee Program.
