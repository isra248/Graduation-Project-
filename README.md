
# EnRoute: A Gamified Productivity Application Inspired by Istanbul's Public Transportation

## 1. Project Overview

| Item | Description |
|---|---|
| **Project Name** | EnRoute |
| **Project Type** | Software Engineering Graduation Project |
| **Application Type** | Cross-platform Mobile Application |
| **Target Users** | People who study, work, or learn new skills |
| **Mobile Development** | Flutter, Dart |
| **Backend Development** | Java |
| **Database** | PostgreSQL |
| **Version Control** | Git, GitHub |

## 2. Project Description

EnRoute is a productivity app that gamifies focus sessions, turning them into virtual adventures influenced by Istanbul’s public transit system. It is intended for individuals who study, work, or acquire new skills and seek a more engaging approach to organize their concentrated efforts.

Instead of showing a focus session as a countdown timer, EnRoute illustrates it as a journey featuring a starting point, a path, interim milestones, and an endpoint.
Users choose a departure station and a destination from an online map influenced by Istanbul's metro, Metrobus, Marmaray, and ferry systems. The chosen path dictates the intended focus time. Throughout the session, the user's virtual experience moves forward from station to station, offering a visual depiction of time and advancement. Qualifying finished sessions grant virtual points and might reveal rewards.

The application also intends to offer session history, fundamental statistics, and a rewards catalog. Upcoming additions might consist of collaborative focus paths, simulated peak hour scenarios, and extra obstacles. These attributes will be created based on project priorities, time constraints, and technical viability.
EnRoute will utilize Flutter and Dart for the mobile app, Java for backend development, and PostgreSQL for data storage. The architecture will be improved throughout system design to determine how the mobile client, backend, and database interact.

The primary objective is to provide a workable minimum viable product (MVP) and assess its usability, dependability, and perceived engagement. The question of whether the journey-based method provides a more captivating experience than a standard timer still requires investigation through testing and user feedback.

## 3. Introduction

Digital devices give people access to learning materials, communication tools and work environments.. They also bring constant notifications distractions from entertainment and frequent switching between tasks. This can make it hard for some people to stay focused over time.

Productivity apps often include features like timers to-do lists and tools to block distractions. These help users stay on track. A timer-based setup may not give the kind of engagement or sense of growth that some users really want.

Gamification is a way to build engaging digital experiences by using goals, progress tracking, feedback and rewards. Its success depends a lot, on how it's used and the situation its applied to.

EnRoute tries out one use of this idea. It turns work into a virtual journey through a transportation network inspired by Istanbul. The app combines focus-time controls with a path that moves forward as users work. It also includes rewards to keep motivation high. The project will look at whether this concept works and how well people respond to the experience it offers.


## 4. Problem Statement

Conventional focus timers provide a straightforward way to allocate time to a task, but they typically emphasize elapsed time and session completion. For users who find this experience repetitive or insufficiently engaging, maintaining a consistent focus routine may remain challenging.

EnRoute addresses the opportunity to explore an alternative way of presenting a focus session through a visual, goal-oriented journey.

The project investigates the following research question:

**Can a journey-based, gamified interface provide a more engaging and usable focus-session experience than a conventional timer interface?**

This question will be explored through the implementation of a working mobile application and an initial user evaluation. EnRoute will not claim to improve productivity unless the evaluation provides supporting evidence.

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
| FR-03 | Session Configuration | Users can review the selected route and planned focus duration before starting. |
| FR-04 | Focus Timer and Journey Progress | The timer tracks elapsed time and updates the virtual journey according to session progress. |
| FR-05 | Session Control | Users can start, pause, resume, or cancel a session according to defined session rules. |
| FR-06 | Session Completion and Rewards | Eligible completed sessions generate rewards once, without duplicate awards. |
| FR-07 | Reward Catalogue | Users can view available virtual rewards and unlock eligible rewards when they have sufficient points. |
| FR-08 | Session History and Statistics | Users can review previous sessions, including duration, route, and completion status. |
| FR-09 | Shared Focus Journeys | If included, users can join a shared journey and view other participants' session states. |
| FR-10 | Challenges | If included, the application supports predefined challenges with explicit completion conditions and reward rules. |

### 6.2 Non-Functional Requirements

The following are initial engineering targets to be validated and refined during implementation and testing.

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

Authentication and cloud persistence will be implemented according to the final system architecture and data requirements.

### 7.2 Features Dependent on Feasibility

The following features may be implemented after the core MVP:

- Shared focus journeys and participant synchronization.
- Simulated rush-hour challenges.
- Additional challenge types and reward conditions.
- Expanded virtual vehicle customization.
- Weekly competitions and additional social features.

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
- Java and PostgreSQL are the planned backend and database technologies.
- Shared journeys may require authentication, synchronization, and additional backend functionality.
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
| 1. Requirements and Research | Review relevant literature, define target users, and refine requirements and scope. | Initial specification and research summary. |
| 2. System Design | Design the application architecture, data model, user flows, and interface prototypes. | Architecture diagrams, data model, and UI designs. |
| 3. Core Implementation | Build route selection, session timing, journey progression, and session-state handling. | Working core application. |
| 4. Rewards and Persistence | Implement points, rewards, history, and the selected storage solution. | Persistent MVP features. |
| 5. Optional Features | Investigate shared journeys and challenges after core functionality is stable. | Additional features where feasible. |
| 6. Testing and Evaluation | Perform functional, usability, timer, persistence, and reliability tests. | Test results and user feedback. |
| 7. Final Documentation | Document architecture, implementation decisions, results, limitations, and future work. | Final report and project deliverables. |

### 9.1 Evaluation Approach

The application will be evaluated in two ways.

**Technical Evaluation**

- Verify route selection and duration calculation.
- Test timer behavior during pause, resume, cancellation, and supported background operation.
- Confirm that completed sessions and rewards are recorded correctly.
- Test data persistence after application restarts.
- Measure response times under documented test conditions.
- Test synchronization and network interruption if shared journeys are implemented.

**User Evaluation**

- Ask participants to complete representative tasks using the application.
- Collect feedback on ease of use, clarity of progress, and the appeal of the journey metaphor.
- Assess whether users understand session duration, completion, and reward rules.
- Identify usability issues and opportunities for improvement.

Any claim that EnRoute improves engagement or productivity will be limited to the evidence collected. An initial user evaluation can reveal usability issues and perceived engagement, but it cannot by itself establish a general causal effect on productivity.

## 10. Initial References

### 10.1 Academic References

1. Sailer, M., & Homner, L. (2020). The Gamification of Learning: A Meta-analysis. *Educational Psychology Review, 32*, 77–112. https://doi.org/10.1007/s10648-019-09498-w

2. Zainuddin, Z., Chu, S. K. W., Shujahat, M., & Perera, C. J. (2020). The Impact of Gamification on Learning and Instruction: A Systematic Review of Empirical Evidence. *Educational Research Review, 30*, 100326. https://doi.org/10.1016/j.edurev.2020.100326

These studies provide background on gamification and learning-related outcomes. They do not directly establish that EnRoute will improve productivity.

### 10.2 Technical References

1. Flutter. [Flutter Documentation](https://docs.flutter.dev/)
2. GitHub. [About Repositories](https://docs.github.com/en/repositories/creating-and-managing-repositories/about-repositories)
3. Java. [Java Documentation](https://docs.oracle.com/en/java/)
4. PostgreSQL. [PostgreSQL Documentation](https://www.postgresql.org/docs/)

## 11. Use Case Diagram

The following diagram illustrates the main interactions between users and the EnRoute system.

![EnRoute Use Case Diagram](Photos/Usecasediagram.png)

