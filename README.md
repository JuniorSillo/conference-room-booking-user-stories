# 👨🏻‍💻 Conference Room Booking System

This repository contains a practice project used to demonstrate professional Git, GitHub, and collaboration workflows. The project simulates a Conference Room Booking System that will be expanded over multiple modules to support learning around documentation, APIs, teamwork, and system handover.

## 📌 Purpose of This Repository

This repository serves as a hands-on environment for:

- Practicing Git and GitHub fundamentals, including branching, committing, and merging.
- Creating and reviewing Pull Requests as a means of structured communication and code review.
- Working with sprint documentation to simulate real-world Agile processes.
- Gradually improving project documentation over time to support onboarding and maintainability.

At this stage, the repository emphasizes process, communication, and foundational setup rather than a fully implemented system. It is designed for trainees and developers to experiment with professional workflows in a low-stakes environment.

## 🗂 Repository Contents

- **README.md** – This comprehensive onboarding and overview document
- **docs/** – Key sprint documentation artefacts
- `user-stories.md` – User stories and acceptance criteria
- `epics.md` – Grouping of stories into logical epics (e.g., Employee Features, Admin Features)
- `estimation.md` – Velocity calculation, team estimation, and story points
- `priority-matrix.md` – Business value vs. effort/complexity prioritization
- `sprint-1-review.md` – Sprint review summary with outcomes and lessons learned
- **LICENSE** – Project license (MIT)
  
As the project evolves, folders like `src/` (source code), `tests/` (unit tests), and `.github/` (workflows and templates) will be added.

## ⚙️ Installation

This project is in early stages and does not require full installation yet. However, for basic setup and to interact with documentation or future code:

### Prerequisites
- Git (version 2.25+ recommended).
- A GitHub account for forking/cloning and collaborating.
- Optional: Node.js (v18+) or Python (v3.10+) if experimenting with prototype code in future iterations.
- Text editor or IDE (e.g., VS Code) for viewing/editing markdown files.

### Quick Setup
1. Clone the repository:
   ```
   git clone https://github.com/JuniorSillo/conference-room-booking-user-stories.git
   cd conference-room-booking-user-stories
   ```
2. (Future: Install dependencies if code is added, e.g., `npm install` or `pip install -r requirements.txt`.)
3. Explore the docs: Open files in `sprint/` or `docs/` to review artefacts.

No database or server setup is needed at this point, but placeholders for Docker or local dev environments will be added later.

## 🚀 Usage

This repository is currently used for:

1. Reviewing and evolving documentation practices to ensure clarity and accessibility.
2. Creating Pull Requests to propose changes, discuss improvements, and collaborate.
3. Simulating Scrum sprints through artefact creation and peer reviews.

Example workflow:
- Fork the repo for personal experiments.
- Create a branch for a new feature or doc update.
- Submit a PR and engage in reviews.

In future modules, usage will expand to running a web app for booking rooms, querying APIs, and testing features.

## 🤝 Contributing

We follow a collaborative, professional workflow to ensure high-quality contributions. Changes are **never** pushed directly to the `main` branch.

### Contribution Workflow
1. **Fork the Repository**: If you're external, fork it to your account.
2. **Create a Branch**: Use descriptive names like `feature/add-api-docs` or `docs/improve-onboarding`.
   ```
   git checkout -b your-branch-name
   ```
3. **Make Changes**: Commit with clear, conventional messages (e.g., `feat: add room booking endpoint`, `docs: update system context`).
4. **Push and Open a Pull Request**:
   - Push: `git push origin your-branch-name`.
   - On GitHub, create a PR with:
     - A descriptive title.
     - Body explaining *why* the change (purpose), *what* was done, and what to review (e.g., "Focus on clarity of instructions").
     - Reference related issues or sprint artefacts.
5. **Request Reviews**: Assign at least one peer/teammate.
6. **Address Feedback**: Iterate based on comments.
7. **Merge**: Once approved, merge into `main` and delete the branch.

Use Pull Requests for all changes – they serve as communication artefacts, documenting intent, decisions, and reviews. For issues, use GitHub Issues with templates (see `.github/ISSUE_TEMPLATE/` for bug reports and feature requests).

## Developer Onboarding (In Progress)
-This project is developed incrementally as part of a Software training program. The purpose of this section is to help new contributors to understand
-What this system is intended to become
-How documentation is organised
-Where to find key project artefacts
-What technologies will be used to develop this project?

### What This System Is Intended to Become
The Conference Room Booking System will grow into a practical web application that helps organizations manage meeting spaces effectively. It will allow employees to check room availability, make reservations, cancel bookings, and avoid double-bookings. Admins will be able to add/edit rooms, oversee usage, and generate basic reports.
The goal is to solve common workplace scheduling pain points while demonstrating clean architecture, good APIs, and maintainable code.

### System Context (High-Level)
The system manages:
- **Room Availability**: Tracking rooms, capacities, and amenities.
- **Booking Requests**: User-initiated reservations with date/time validation.
- **Conflict Prevention**: Real-time checks to avoid overlaps.
- **Administration Oversight**: Dashboards for approvals, cancellations, and reports.
- **(Future Expansions)**: Integrations like calendar sync, notifications, or mobile access.

Major components (high-level):
- **Frontend**: User interface (e.g., React or HTML/JS for forms and calendars).
- **Backend**: Logic server (e.g., Node.js/Express or Python/Django for APIs and validation).
- **Database**: Storage (e.g., PostgreSQL or MongoDB for bookings and users).
- **Authentication**: Basic user login (e.g., JWT or sessions).

At this stage, the system is primarily documented through sprint artefacts; code implementation starts in later modules.

### How Documentation Is Organized
- **Core Docs**: This README for overview and onboarding.
- **Sprint Artefacts**: In `sprint/` – user stories, planning docs, retrospectives.
- **Technical Docs**: In `docs/` – architecture diagrams, API specs (e.g., OpenAPI), and markdown files from sprints.

### Where to Find Key Project Artefacts
- User stories and requirements: `sprint/sprint-1/user-stories.md`.
- Architecture overview: `docs/architecture.md`.
- API specifications: `docs/api-spec.md` (placeholder until implemented).
- Reflection files: Root level, e.g., `documentation-and-collaboration-reflection.md`.

### Technologies Used/Planned
- **Version Control**: Git + GitHub.
- **Documentation**: Markdown for all artefacts.
- **(Future Tech Stack)**: JavaScript/Node.js (or Python), SQL database, Docker for deployment, Jest/Pytest for testing.

Start by reading this README, then explore `sprint/` folders. Aim to contribute via a small PR to get familiar.

## Project Documentation

This repository contains sprint documentation created during Scrum simulations:
- **sprint-1/**: Sprint planning, execution, and review artefacts (e.g., backlog, daily standups, demo notes).

These represent real project evolution, review them to understand decisions and progress.

## Upcoming Documentation

The following sections will be added as the project evolves:
- **API Documentation**: Full endpoints via Swagger/OpenAPI.
- **Runtime Instructions**: Docker Compose for local/prod deployment.
- **Developer Setup**: Detailed env vars, scripts, and CI/CD workflows.
- **Testing Guide**: How to run unit/integration tests.
- **Security and Best Practices**: Guidelines on auth, validation, and scalability.

## LICENSE

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## ✍️ Author

Moeketsi Junior Sillo: sillojunior8@gmail.com
Created as part of Software Development Trainee Program.

---
