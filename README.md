
# EnRoute: A Gamified Productivity Application Inspired by Istanbul's Public Transportation

## 1. Project Overview

| Item | Description |
|---|---|
| Project Name | EnRoute |
| Project Type | Software Engineering Graduation Project |
| Application Type | Cross-platform mobile application |
| Target Users | People who study, work, or learn new skills |
| Planned Technologies | Flutter, Dart|
| Backend / Database | Java, PostgerSQL |

## 2. Project Description

EnRoute is a gamified productivity app that converts personal focus sessions into virtual adventures influenced by Istanbul's public transit system. It is intended for individuals who study, work, or acquire new skills and seek a more interactive method to structure concentrated tasks. Instead of showing a session just as a countdown timer, EnRoute illustrates it as a journey that includes a beginning, a path, noticeable advancement, and an endpoint.

At the beginning of a session, users select a departure station and a destination on a virtual map inspired by Istanbul's metro, Metrobus, Marmaray, and ferry networks. The application uses the selected route to determine a planned focus duration. As time passes, the user's virtual journey progresses from one station to the next, making the passage of time visible through movement along the route. Completing a session allows users to earn virtual points and collect station-based rewards.

The application combines this journey-based interface with a reward system intended to encourage continued participation. Users can accumulate points, unlock virtual rewards, track completed journeys, and review basic session statistics. The transportation theme provides a consistent structure for these features: routes represent goals, stations represent milestones, and destinations represent completed focus sessions. The system does not require users to travel physically or connect to live transportation services.

EnRoute is also intended to explore the social dimension of focused work. A planned feature will allow users to join shared focus journeys with friends or other participants and see their session progress. Optional challenges, such as simulated rush-hour events or sessions with additional completion conditions, may introduce variety and provide further incentives. These events will be simulated within the application rather than based on actual traffic or public transportation conditions.

The project will initially prioritize a functional minimum viable product (MVP) containing route selection, focus-session management, journey visualization, rewards, and session history. Shared journeys and additional challenges will be implemented according to available time and technical feasibility. The application will be developed using Flutter and Dart, with version control managed through Git and GitHub. Backend and database technologies will be selected after evaluating the requirements for authentication, data persistence, and synchronization between users.

The central purpose of EnRoute is to investigate whether representing focus sessions as interactive journeys can provide a more engaging experience than a conventional timer. Its effectiveness will not be assumed in advance. The completed application will be evaluated through functional testing and user feedback, with particular attention to usability, engagement, reliability, and the clarity of session progress.

## 3. Introduction

Digital devices provide convenient access to learning resources, communication tools, and work environments. However, the same devices can also expose users to notifications, entertainment, and frequent task switching. Maintaining a consistent focus routine can therefore be challenging for some users.

Many productivity applications provide timers, task lists, or blocking mechanisms to help users structure their work. Although these tools address important parts of the problem, their interfaces do not always provide a strong sense of progression or a rewarding experience throughout a session.

Gamification offers one possible approach to designing more engaging digital experiences. By incorporating goals, feedback, progress indicators, and rewards, applications can encourage users to interact with a system over time. However, the effectiveness of these elements depends on their design, context, and implementation.

EnRoute explores a specific application of this approach: representing focused work as a virtual journey through a familiar public transportation network. It combines session timing and progress visualization with a route-based interface and a system of virtual rewards. The project will investigate the feasibility of this concept and evaluate how users respond to the resulting experience.

## 4. Problem Statement

Conventional focus timers can help users allocate time to a task, but they often represent a session primarily through elapsed time and a completion notification. For users who find this experience repetitive or insufficiently engaging, maintaining a consistent focus routine may remain difficult.

The problem addressed by EnRoute is therefore not the absence of timers, but the opportunity to explore a different way of presenting and experiencing a focus session.

The project investigates the following question:

**Can a journey-based, gamified interface provide a more engaging and usable focus-session experience than a conventional timer interface?**

This question will be explored through the implementation of a working mobile application and an initial evaluation with users. EnRoute will not claim to improve productivity unless the evaluation provides supporting evidence.

## 5. Motivation and Objectives

### 5.1 Motivation

A journey has a beginning, a path, intermediate milestones, and an endpoint. These elements offer a natural way to visualize progress through a period of focused work.

Istanbul's public transportation network provides a recognizable structure for this concept. Stations can represent milestones, routes can represent planned sessions, and reaching a destination can represent completion. This metaphor gives the application a consistent visual and functional identity rather than adding unrelated rewards to a standard timer.

The motivation behind EnRoute is to explore whether this representation can make focused work feel more structured, visible, and engaging while remaining practical for everyday use.

### 5.2 Objectives

The project aims to:

1. Design and implement a cross-platform mobile application using Flutter and Dart.
2. Develop a virtual transportation map that supports departure and destination selection.
3. Implement a reliable focus timer linked to virtual journey progression.
4. Create a reward system based on eligible completed sessions.
5. Provide session history and basic statistics.
6. Investigate the feasibility of shared focus journeys and synchronized progress.
7. Evaluate the application's usability, technical reliability, and perceived engagement through testing and user feedback.
8. Document the system's architecture, requirements, implementation, testing, and limitations.

## 6. Initial Software Requirements

### 6.1 Functional Requirements

| ID | Requirement | Acceptance Criteria |
|---|---|---|
| FR-01 | User Profile | Users can access their profile and view their points, completed sessions, and collected rewards. |
| FR-02 | Route Selection | Users can select a valid departure and destination from the predefined virtual transportation network. |
| FR-03 | Session Configuration | Before starting, users can review the selected route and its planned focus duration. |
| FR-04 | Focus Timer and Journey Progress | The timer tracks elapsed time and updates the virtual journey according to the session's progress. |
| FR-05 | Session Control | Users can start, pause, resume, or cancel a session according to the defined session rules. |
| FR-06 | Session Completion and Rewards | Eligible completed sessions generate the defined rewards once, without duplicate awards. |
| FR-07 | Reward Catalogue | Users can view available virtual rewards and unlock eligible rewards when they have sufficient points. |
| FR-08 | Session History and Statistics | Users can review previous sessions, including their duration, route, and completion status. |
| FR-09 | Shared Focus Journeys | If included in the MVP, users can join a shared journey and view other participants' session states. |
| FR-10 | Challenges | If included, the application supports predefined challenges with explicit completion conditions and reward rules. |

### 6.2 Non-Functional Requirements

The following are initial engineering targets. They must be validated and refined during implementation and testing.

| ID | Requirement | Initial Acceptance Target |
|---|---|---|
| NFR-01 | Usability | A returning user can start a focus session within three main actions from the home screen. |
| NFR-02 | Performance | The home screen and common interactions respond within two seconds under normal test conditions. |
| NFR-03 | Timer Accuracy | The timer remains within two seconds of the expected duration during a 60-minute test, including supported background operation. |
| NFR-04 | Reliability | A session completion event cannot generate duplicate session records or rewards. |
| NFR-05 | Data Persistence | Saved profile, history, and reward data remain available after an application restart. |
| NFR-06 | Security | Authentication credentials and protected user data are handled using appropriate security practices. |
| NFR-07 | Privacy | Private profile and session data are accessible only to authorized users, except for information intentionally shared. |
| NFR-08 | Compatibility | The application works on the selected target Android and/or iOS versions and supported screen sizes. |
| NFR-09 | Maintainability | User interface, session management, reward logic, and data access are separated into maintainable components. |
| NFR-10 | Network Resilience | If shared journeys are implemented, temporary network loss is communicated clearly and does not unnecessarily reset the local timer. |

## 7. Project Scope

### 7.1 Planned MVP

The first functional version will prioritize:

- Core application navigation and user profile functionality.
- A predefined virtual transportation network.
- Departure and destination selection.
- Focus-session timing and visual journey progression.
- Session start, pause, resume, cancellation, and completion rules.
- Virtual points and a basic reward catalogue.
- Persistent session history and basic statistics.
- Essential testing and documentation.

Authentication and cloud persistence will be implemented if required by the final architecture. Their exact implementation will depend on the backend and database selected during system design.

### 7.2 Features Dependent on Feasibility

The following features may be implemented after the core MVP:

- Shared focus journeys and participant synchronization.
- Simulated rush-hour challenges.
- Additional challenge types and reward conditions.
- Expanded virtual vehicle customization.
- Weekly competitions and more advanced social features.

### 7.3 Out of Scope

The initial project will not include:

- Live public transportation tracking or real-time arrival predictions.
- Integration with official Istanbulkart payment or ticketing services.
- Actual public transportation bookings or payments.
- An advanced messaging platform or full social network.
- Claims of scientifically proven productivity improvement without appropriate evaluation.

## 8. Constraints and Assumptions

### 8.1 Constraints

- The project must be completed within the graduation-project timeline.
- Development capacity, testing resources, and participant availability are limited.
- Flutter and Dart are the planned mobile development technologies.
- Shared journeys may require a backend, database, authentication, and synchronization.
- The initial transportation network will be predefined rather than dependent on live transit services.
- Optional features must not compromise the implementation and testing of core functionality.

### 8.2 Assumptions to Validate

- Some users may prefer a visual, goal-oriented focus experience to a conventional timer.
- A predefined transportation network will be sufficient to demonstrate the core concept.
- Virtual rewards may encourage users to return to the application, although this must be tested.
- Shared journeys may be useful to users who prefer working alongside others.
- Users can understand the relationship between route length, planned duration, and session completion without extensive instruction.

These assumptions are hypotheses for design and evaluation, not established findings.

## 9. Development Plan and Evaluation

The project will follow an iterative development process. Each stage will produce a testable result before additional complexity is introduced.

| Phase | Main Activities | Expected Output |
|---|---|---|
| 1. Requirements and Research | Review relevant literature, define target users, refine requirements and scope. | Initial specification and research summary. |
| 2. System Design | Design the application architecture, data model, user flows, and interface prototypes. | Architecture diagrams, data model, and UI designs. |
| 3. Core Implementation | Build route selection, session timing, journey progression, and session-state handling. | Working core application. |
| 4. Rewards and Persistence | Implement points, rewards, history, and the selected storage solution. | Persistent MVP features. |
| 5. Optional Features | Investigate shared journeys and challenges after core functionality is stable. | Additional features where feasible. |
| 6. Testing and Evaluation | Perform functional, usability, timer, persistence, and reliability tests. | Test results and user feedback. |
| 7. Final Documentation | Document architecture, implementation decisions, results, limitations, and future work. | Final report and project deliverables. |

### 9.1 Evaluation Approach

The application will be evaluated in two distinct ways.

**Technical evaluation**
- Verify that route selection and duration calculation behave as specified.
- Test timer behavior during pause, resume, cancellation, and supported background operation.
- Confirm that completed sessions and rewards are recorded correctly.
- Test data persistence after application restarts.
- Measure response times under documented test conditions.
- Test synchronization and network interruption if shared journeys are implemented.

**User evaluation**
- Ask participants to complete representative tasks using the application.
- Collect feedback on ease of use, clarity of progress, and the appeal of the journey metaphor.
- Assess whether users understand how session duration, completion, and rewards work.
- Identify usability issues and opportunities for improvement.

Any claim that EnRoute improves engagement or productivity will be limited to the evidence collected. An initial user evaluation can reveal usability issues and perceived engagement, but it cannot by itself establish a general causal effect on productivity.

## 10. Initial References

### 10.1 Academic References

1. Sailer, M., & Homner, L. (2020). The Gamification of Learning: A Meta-analysis. *Educational Psychology Review, 32*, 77–112. https://doi.org/10.1007/s10648-019-09498-w

2. Zainuddin, Z., Chu, S. K. W., Shujahat, M., & Perera, C. J. (2020). The Impact of Gamification on Learning and Instruction: A Systematic Review of Empirical Evidence. *Educational Research Review, 30*, 100326. https://doi.org/10.1016/j.edurev.2020.100326

These studies provide background on gamification and learning-related outcomes. They do not directly establish that EnRoute will improve productivity.

### 10.2 Technical References

1. Flutter. *Flutter Documentation*. https://docs.flutter.dev/
2. GitHub. *About Repositories*. https://docs.github.com/en/repositories/creating-and-managing-repositories/about-repositories

## 11. Repository and Project Progress

**GitHub Repository:** [Add the actual repository URL]

Development progress will be tracked through meaningful commits, with changes grouped by feature or task. The repository will contain the source code, README, and relevant project documentation.

