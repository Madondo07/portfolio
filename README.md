# Dumisane Madondo

**Application Development Student**  
Cape Town, South Africa  
📧 230949703@mycput.ac.za | 📱 076 045 0332 | [LinkedIn](https://www.linkedin.com/in/dumisane-madondo-34261626b) | [GitHub](https://github.com/Madondo07)

---

## 🎯 Objective

Final-year Diploma in ICT: Application Development student at CPUT, currently completing **Work Integrated Learning at Demand Academy | CAPACITI** as lead backend developer on a team-built Candidate Operations and Attendance Platform. Seeking a **graduate software development opportunity** where I can apply my full-stack and backend skills, work in agile teams, and contribute product thinking alongside technical delivery. Dedicated to creativity, problem-solving and collaboration, with a goal of continuously expanding my expertise in modern software practices.

---

## 🎓 Education

- **Madisong Secondary School** — National Senior Certificate (2021)  
- **Cape Peninsula University of Technology** — Higher Certificate in ICT (2023)  
- **Cape Peninsula University of Technology** — Diploma in ICT: Application Development (2024 – 2026)

---

## 💻 Technical Skills

- Programming: **Java & Python**  
- Backend: **Spring Boot, REST APIs, JWT authentication, Laravel**  
- Database Design: **MySQL, PostgreSQL (Supabase)**  
- Frontend: **HTML, CSS & JavaScript**  
- Data Structures  
- Version Control: **Git & GitHub**  
- Deployment: **Vercel**

---

## 📂 Projects

- **CAPACITI Candidate Operations and Attendance Platform**  
  Team-built platform managing daily attendance for On-Site and Work-From-Home candidates, with timed check-ins, location security and an AI quality gate. I am lead backend developer (Java, Spring Boot, Supabase PostgreSQL).

- **Enrollment System**  
  Client-server application for managing student course enrollments.

- **Clinic Booking System**  
  Web-based system for patient management, appointment scheduling, and queue management.

- **SafeRide**  
  Ride-sharing application focusing on secure authentication, booking, and ride management.

---

# 📘 Assessment 1

## ✨ Reflections (STAR Method)

**📃Markdown Coding**  
    **Situation:** Documenting project work in Markdown.  
    **Task:** Create clean, readable documentation.  
    **Action:** Learned and applied line/divider syntax.  
    **Result:** Improved readability and structure.  
    **Reflection:** Discovering how to set up lines was new and interesting, showing me how formatting elevates documentation.

**🎥 Mock Interview Video**  
    **Situation:** Required to record and upload a mock interview.  
    **Task:** Simulate a real interview and share it online.  
    **Action:** Prepared responses, recorded video, overcame upload size limits.  
    **Result:** Video displayed with full playback controls.  
    **Reflection:** Seeing the controllers made the video interactive; the challenge of file limits taught me patience and problem-solving.

**💻 GitHub Pages**  
    **Situation:** Needed to publish my portfolio online.  
    **Task:** Make projects accessible in a professional format.  
    **Action:** Set up GitHub Pages, linked repos, customized layout.  
    **Result:** Portfolio became publicly visible and professional.  
    **Reflection:** Although I knew about GitHub Pages, I didn’t expect it to be formally required. This reinforced the importance of presentation in industry-standard tools.

---

# 📗 Assessment 2

## 🗂️ Agile Project Management

**Project:** CAPACITI Candidate Operations and Attendance Platform (Work Integrated Learning, CAPACITI)  
**My role:** Lead Backend Developer  
**Delivery date:** originally 6 November 2026, brought forward to 29 October 2026

An internal platform that manages daily attendance for CAPACITI candidates in On-Site and Work-From-Home models, with timed check-ins, location security, an AI quality gate and three roles: candidate, tech champion and admin.

---

### 🤝 Agile Team Charter

| Element | Content |
|---|---|
| Purpose | Replace manual attendance tracking with a role-based platform for candidates, tech champions and admins |
| Product Owner | CAPACITI |
| Scrum Master | Omphile Rantswele (Mentor) |
| Development team | Dumisane Madondo, Anita Ndabangaye, Siphokazi Lekena, Abram, Cherish |
| Values | Accountability for own slice, transparency about blockers, protecting candidate data, backend as the single source of truth |
| Working agreements | Daily stand-up every morning before project work, with Cherish taking notes. Contracts agreed before coding. Ownership by file, with the lead owning shared files (config, security, exception, util, pom, properties). Branching: `main` (demo-ready), `develop` (integration), `feature/<entity>` per member. Pull requests reviewed by the lead. Secrets kept in environment variables and shared privately. |
| Definition of Done | Slice implemented on its feature branch, compiles, merged into `develop` through a reviewed pull request, aligned with the agreed API contract |
| Boundaries | No secrets in Git. Members edit only files they own. The frontend uses backend field names, and features the backend lacks are marked mock-only. |
| Communication | Teams messages, morning stand-ups, Bruno collection for API checks |
| Key dates | Internal deadline 27 Oct, buffer 28 Oct, final delivery 29 Oct 2026 |

<!-- Evidence: add a screenshot of the branching rules or Teams ownership message -->
<!-- ![Team charter evidence](images/agile/charter.png) -->

**🤝 Reflection: Agile Team Charter**  
    **Situation:** I joined a five-member CAPACITI team to build the attendance platform, and the delivery date moved from 6 November to 29 October, leaving about eight days to build.  
    **Task:** As lead backend developer, I needed working agreements that let five people build in parallel without conflicts.  
    **Action:** On 19 and 20 October I put in place ownership by file, per-member feature branches, pull request reviews by me, contracts agreed before coding, secrets in environment variables, and a daily morning stand-up with notes taken by Cherish.  
    **Result:** Members built their slices without overwriting each other and `develop` stayed stable. However, a Supabase secret still reached a commit and was blocked by GitHub push protection.  
    **Reflection:** The concrete agreements, such as who owns which file and which branch to use, worked best. The secret incident showed that "secrets in environment variables" had to be enforced from day one rather than assumed. Next time I would write the charter before any code and add a rule on pinning framework versions, since Spring Boot 4.1.1 cost us time. The charter links to the other four topics: its working agreements created the stand-ups in the logbook, and its ownership rules decided how stories were split into tasks.

---

### 📝 User Stories and Tasks

| ID | User story | Tasks | Owner | Status |
|---|---|---|---|---|
| US1 | As a candidate, I want to clock in and out so that my daily attendance is recorded | Attendance entity and endpoints; status engine (arrival and departure stored separately); on-site check against campus IP whitelist | Anita | Done |
| US2 | As a candidate, I want my location verified so that on-site attendance is genuine | Geofence and location verification; IP whitelist; trusted proxy handling | Anita | Done (proxy setting to do) |
| US3 | As a candidate, I want to answer three timed check-ins so that I show I am working | Window calculator; prompt generator; quality attempts; Gemini client and AI quality gate | Siphokazi | Done |
| US4 | As a candidate, I want to apply for WFH so that I can work remotely when approved | WFH request entity and endpoints; approval flow | Abram | Done |
| US5 | As a candidate, I want to log blockers and IT issues so that they get resolved | Support ticket entity and endpoints; blocker queue; prolonged-ticket scheduler | Abram | Done |
| US6 | As a candidate, I want to view my scorecards so that I can see my progress | Assessment and ScorecardEntry entities; endpoints; candidate UI; database script 12 | Anita, Cherish | Done (script 12 in progress) |
| US7 | As a tech champion, I want to monitor attendance and approve or reject WFH so that I can manage my group | Dashboards; WFH approval endpoints; excuse lateness; resolve tickets | Cherish, Abram | Done |
| US8 | As a tech champion, I want to score candidates so that I can give feedback | Mentor Scorecards backend and UI; group defined by `users.champion_id` | Anita | Done |
| US9 | As an admin, I want to manage users, the IP whitelist and the audit log so that the system stays secure | User management; IP whitelist; audit log; reports | Dumisane, Anita, Cherish | Done |
| US10 | As an admin, I want automated reports and Teams alerts so that I do not chase data manually | Attendance and prompt schedulers; reports; Teams webhook client; signed file links | Cherish | Done (live Teams test to do) |
| US11 | As any user, I want role-based login so that I only see what my role allows | Users and login; JWT service and filter; BCrypt; role-based security config; JSON 401/403 handlers | Dumisane | Done |

<!-- Evidence: add a Swagger or Bruno screenshot showing the endpoints for one story -->
<!-- ![User stories evidence](images/agile/user-stories.png) -->

**📝 Reflection: User Stories and Tasks**  
    **Situation:** The team built a frontend-first prototype without Figma wireframes, and the screens included cohort, stream, candidate ID, notifications and break buttons that the backend did not have.  
    **Task:** Define the user stories as the real source of truth for what the platform should do.  
    **Action:** I turned the needs of the three roles into eleven stories and split them into backend slices owned by one member each, using the backend naming as the contract. For example, US3 (timed check-ins) became the window calculator, prompt generator and Gemini quality gate for M3.  
    **Result:** Every member had specific, testable tasks and the slices were implemented. But the stories had no formal acceptance criteria, so the User entity did not match the users table and the mismatch only surfaced during integration.  
    **Reflection:** Writing stories after the prototype cost us rework. Next time I would write the stories first and base the database scripts on them, with acceptance criteria for each. The stories feed directly into the product backlog, where each became a prioritised item.

---

### 📋 Product Backlog

| Priority | Item | Type | Owner | Status |
|---|---|---|---|---|
| 1 | Database schema, RLS and storage policies in Supabase | Feature | Dumisane | Done |
| 2 | Role-based login with JWT and user management | Feature | Dumisane | Done |
| 3 | Attendance clock-in/out and status engine | Feature | Anita | Done |
| 4 | Location security (IP whitelist and geofence) | Feature | Anita | Done |
| 5 | Timed check-ins with AI quality gate | Feature | Siphokazi | Done |
| 6 | WFH requests and approval | Feature | Abram | Done |
| 7 | Support tickets, blockers and prolonged scheduler | Feature | Abram | Done |
| 8 | Dashboards, reports, schedulers, Teams alerts | Feature | Cherish | Done |
| 9 | Frontend for all three roles | Feature | Frontend team | Done (rebuilt from AI Studio design) |
| 10 | Mentor Scorecards | Feature | Anita | Done |
| 11 | Fix Supabase smoke test (missing PostgreSQL driver) | Bug | Dumisane | In progress |
| 12 | Rotate exposed secrets and complete GitHub push | Bug | Dumisane | In progress |
| 13 | Wire every frontend screen to real endpoints | Improvement | Frontend team | In progress |
| 14 | Run scorecards script 12 and create storage buckets | Improvement | Cherish | In progress |
| 15 | Trust X-Forwarded-For only from a trusted proxy | Improvement | Dumisane | To do |
| 16 | End-to-end tests for all three roles; live Gemini and Teams tests | Testing | Team | To do |
| 17 | Update presentation script to match the build | Improvement | Team | To do |
| 18 | Docker and deployment | Improvement | Dumisane | To do |

<!-- Evidence: add a screenshot of the backlog or board -->
<!-- ![Product backlog evidence](images/agile/product-backlog.png) -->

**📋 Reflection: Product Backlog**  
    **Situation:** With the delivery date moved to 29 October, the team had very little time and could not build everything.  
    **Task:** Decide what to build first and keep scope under control.  
    **Action:** I prioritised by dependency, so the database and authentication came first and the AI gate and schedulers later. I accepted Mentor Scorecards as a late extra only after the core flows were complete, and I marked frontend features the backend lacked as mock-only instead of adding them to the backlog.  
    **Result:** All core features were implemented and scope stayed controlled. Bugs such as the smoke test and the secret rotation entered the backlog late, after they had already blocked us, and script 12 for the scorecards remained unconfirmed.  
    **Reflection:** Prioritising by dependency worked well under time pressure, but adding a late feature carried a real risk. Next time I would log technical risks as backlog items from day one. The backlog feeds the sprint backlog, where the top items were pulled into a sprint.

---

### 🏃 Sprint Backlog

**Sprint 3: Backend Feature Slices (20 to 25 Oct)**  
**Sprint goal:** Each member delivers their slice end to end on the agreed contracts.

| Item | Tasks | Owner | Status |
|---|---|---|---|
| Users, login and auth | User management; JWT login; audit log | Dumisane | Done |
| Attendance and location | Campus and IP whitelist; attendance; status engine; geofence | Anita | Done |
| Timed check-ins | Window calculator; prompt generator; Gemini client; quality gate | Siphokazi | Done |
| WFH and support | WFH requests and approval; tickets; blocker queue; prolonged scheduler | Abram | Done |
| Dashboards and automation | Dashboards; reports; schedulers; Teams client; signed file links | Cherish | Done |
| Demo data | Demo data seeder | Lead | Done |
| Live integration tests | Gemini and Teams payload checks | Team | Carried over to Sprint 5 |

**Sprint 5: Extra Feature and Hardening (26 to 29 Oct)**  
**Sprint goal:** A tested, demonstrable platform for 29 Oct.

| Item | Status |
|---|---|
| Mentor Scorecards backend and UI | Done |
| Script 12 and storage buckets | In progress |
| Wire frontend to real endpoints | In progress |
| End-to-end test of all three roles | To do |
| Update presentation script | To do |

<!-- Evidence: add a screenshot of the sprint board showing the sprint goal -->
<!-- ![Sprint backlog evidence](images/agile/sprint-backlog.png) -->

**🏃 Reflection: Sprint Backlog**  
    **Situation:** Sprint 3 ran from 20 to 25 October, with five members each owning a backend slice.  
    **Task:** Deliver every slice end to end on the agreed contracts.  
    **Action:** I agreed contracts and ownership before the sprint started, so all five slices were built in parallel, and I used the morning stand-ups to spot blockers early.  
    **Result:** All five slices were implemented. When they came together we hit compile errors from mismatched contracts, such as `Role` versus `UserRole` and `findByEmail` versus `findByEmailIgnoreCase`, and Spring Boot 4.1.1 caused further problems. This cost about a day of integration fixes, and the live Gemini and Teams tests carried over into Sprint 5.  
    **Reflection:** A clear sprint goal and agreed ownership made parallel work possible, but integrating only at the end was a mistake. Next time I would add an integration checkpoint halfway through the sprint. The sprint backlog connects to the logbook, because the daily stand-ups recorded how each task moved.

---

### 📓 Agile Logbook

#### Taskboard (as at 26 Oct 2026)

| Sprint | Product Backlog | In Progress | Completed |
|---|---|---|---|
| Sprint 0: Prototype (frontend first) | | | Role-based screens on sample data<br>12-slide prototype presentation script<br>Prototype delivered |
| Sprint 1: Planning and Foundation (19 to 21 Oct) | | | Business rules and shift windows<br>Script vs build gap analysis<br>Backend plan, ownership split, timeline<br>Spring Boot skeleton and Git branching<br>Exception package, Helper, TimeUtil, ten enums<br>Copilot base and per-member prompts |
| Sprint 2: Database and Security (21 to 22 Oct) | | Supabase smoke test<br>Storage buckets | 8-table schema, RLS and storage policies<br>Security, CORS, JWT filter and handlers<br>`/api/v1` standard; Spring Boot 3.5.16<br>Secrets moved to environment variables |
| Sprint 3: Backend Feature Slices (20 to 25 Oct) | | Live Gemini and Teams testing | Auth and users<br>Attendance, location, status engine<br>Check-ins and AI quality gate<br>WFH and support tickets<br>Dashboards, reports, schedulers, Teams client<br>Demo data seeder |
| Sprint 4: Integration and Frontend Alignment (22 to 26 Oct) | | Wire frontend to real endpoints<br>Secret rotation and GitHub push | Compile, config and merge fixes<br>User entity aligned with table<br>Frontend rebuilt from AI Studio design |
| Sprint 5: Hardening (26 to 29 Oct) | End-to-end tests for all roles<br>Update presentation script<br>X-Forwarded-For setting<br>Docker and deployment | Scorecards script 12 | Mentor Scorecards backend and UI |

#### Walkthrough

| Question | Answer |
|---|---|
| What do we need to do to advance this piece of work? | Confirm the Supabase connection and schema validation, wire every frontend screen to the real endpoints, and run end-to-end tests for the candidate, tech champion and admin roles. The scorecards database script (script 12) must also be run before Mentor Scorecards can be validated. |
| Is anyone working on anything that is not on the board? | Mentor Scorecards was added late as an extra feature, outside the original plan. |
| What do we need to finish as a team? | Confirm the secrets were rotated and the push to GitHub succeeded, create the storage buckets, update the presentation script to match the final build, and prepare for the internal deadline on 27 Oct (buffer 28 Oct) and the final delivery on 29 Oct. |
| Are there any bottlenecks or blockers to the flow of work? | Resolved: Spring Boot 4.1.1 caused compile errors (pinned to 3.5.16), a JDK older than 21 blocked builds, a duplicate main class and merge conflicts needed fixing, and the User entity did not match the users table. Still open: the Supabase smoke test (missing PostgreSQL driver), GitHub push protection blocking a secret in `.env.example`, and live testing of the Gemini and Teams integrations. |

#### Daily Stand-ups

| Date | What did I complete since the last stand-up? | What am I planning to complete next? | Impediments |
|---|---|---|---|
| Mon 19 Oct 2026 | Compared the prototype script against the build and drafted the backend plan, timeline and ownership split. Created the Spring Boot skeleton with the exception package. Prepared the first prompts for Member 1. | Write the base Copilot prompt and the prompts for Members 2 to 5. | The delivery date was brought forward from 6 November to 29 October, which left no time for Figma wireframes. The frontend also showed fields the backend did not have. |
| Tue 20 Oct 2026 | Finished the base Copilot prompt and the per-member prompts so each member could start their slice. | Agree the controller style, then set up the config classes, the location stub and the demo data prompt. | No blockers recorded. The risk was members' code not matching each other's contracts. |
| Wed 21 Oct 2026 | Set the controller style, config prompts, location stub and demo data prompt. Decided on the `/api/v1` path standard. Pinned Spring Boot to 3.5. | Set up the Supabase database, the RLS and storage scripts, and the connection. | Spring Boot 4.1.1 caused Jackson and WebFlux incompatibilities with our Boot 3 assumptions. Fixed by pinning to 3.5.16. |
| Thu 22 Oct 2026 | Created the 8-table schema, RLS, deny policies and the storage policy in Supabase. Wrote the Member 5 instructions and ran the first smoke test. Fixed compile errors, deleted a duplicate main class and resolved merge conflicts. Aligned the User entity with the table. | Prepare the backend summaries and the frontend design prompts. | The smoke test used the dashboard URL instead of the JDBC URL, then failed on a missing PostgreSQL driver. GitHub push protection blocked a Supabase secret in `.env.example`, so the key had to be rotated and the commits squashed. |
| Fri 23 Oct 2026 | Wrote the backend summaries and the frontend design and polish prompts. Found that the candidate dashboard did not match the backend. Replaced the frontend with the Google AI Studio build, aligned to the backend types, with mock-only features marked. | Plan Mentor Scorecards and prepare progress reports. | The frontend did not follow the design and fonts did not load, which caused the rebuild. Wiring screens to real endpoints is still open. |
| Mon 26 Oct 2026 | Planned and delivered Mentor Scorecards (backend and UI, Member 2). Recapped the check-in rules and wrote the progress reports. | Confirm the smoke test and the GitHub push, run script 12, and start end-to-end testing for the 27 Oct internal deadline. | Script 12, the storage buckets and the final GitHub push are all unconfirmed. Live Gemini and Teams testing has not been done. |

<!-- Evidence: add a photo or screenshot of the stand-up notes -->
<!-- ![Stand-up notes evidence](images/agile/standup-notes.png) -->

**📓 Reflection: Agile Logbook**  
    **Situation:** The team held a stand-up every morning before working on the platform, and Cherish took notes of each session.  
    **Task:** Keep a record of what was completed, planned and blocked, so progress could be traced.  
    **Action:** I logged each stand-up from 19 to 26 October using the template's three questions, alongside a taskboard and a walkthrough of where the team stood.  
    **Result:** The log shows what went well, such as agreeing contracts and file ownership early and recovering quickly from build errors. It also exposes what did not: the frontend-first approach created rework, I pinned the framework version late, and a secret reached a commit. The moved deadline is visible in the earliest entries and explains the pressure behind many later decisions.  
    **Reflection:** Reading the log back, I noticed we often discussed blockers but rarely reviewed how we worked, so a proper retrospective would have helped. Next time I would pin versions on day one, sketch wireframes even without Figma, and hold a short retrospective after each sprint. The logbook ties the other four topics together: the charter set the stand-up routine, and the stories, backlog and sprint are what the entries record.

---

### 🔗 How the Five Pieces Connect

The charter set the rules, such as file ownership, branching and the daily stand-up. The user stories turned the platform's purpose into work each member could own, and the product backlog ranked that work by dependency. The sprint backlog pulled the top items into a sprint with a clear goal, and the logbook recorded what actually happened each morning. Gaps in the earlier pieces, such as missing acceptance criteria and a late-pinned framework version, show up as blockers in the logbook. That loop is what I would carry into my next project: write the charter and stories first, pin versions on day one, and hold a retrospective after every sprint.

---

## 📌 References

- **Mr. Omphile Rantswele** — Tech Champ/Mentor <br>
  📧 omphile.rantswele@capaciti.org.za
- **Mr. Kruben Naidoo** — Senior Lecturer  
  📧 naidook@cput.ac.za

  ### 🎥 Mock Interview

<video width="600" controls>
  <source src="Mock Interview Video.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>
