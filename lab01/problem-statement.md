# Problem statement · ITC Club Hub (v0.1, 2026-10-20)

## Problem
The problem of fragmented club registration, unorganized event scheduling, and manual attendance tracking affects ITC students, club leaders, and institute administrators; the impact of which is overcrowded event venues, lost participation records, missed notifications, and high administrative overhead in Telegram chat groups. A successful solution would provide a centralized platform for discovering clubs, registering for events with capacity enforcement, and tracking official student involvement.

## Vision
For ITC students and club organizers who struggle with chaotic event coordination, ITC Club Hub is a centralized management system that simplifies club membership, automates event registration, and tracks attendance records. Unlike ad-hoc Telegram groups and paper sign-up sheets, our product offers real-time capacity management, verified attendance logs, and clear role-based access for students and administrators.

## Today's workaround
Currently, club leaders rely on public Telegram chat groups and Google Forms for event announcements and sign-ups. Attendance is taken manually on paper or spreadsheet lists, leading to duplicate registrations, venue overbooking, untracked cancellations, and no centralized record for university administration.

## Scope
- Built in C++ this semester:
  - Core C++ console management application for processing user authentications, event registrations, attendance logging, and file I/O data persistence.
  - Business logic rules (capacity enforcement, duplicate registration prevention, role-based permissions).
- Modelled only (web and mobile):
  - UI/UX mockups for mobile app student dashboard and web browser admin portal.
  - REST API endpoint specifications for syncing mobile frontend with C++ backend.
- Out of scope:
  - Real-time payment gateway integration for paid club fees.
  - Automated SMS/Push notification servers.
  - Full institute-wide single sign-on (SSO) OAuth server integration.