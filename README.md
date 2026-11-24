# DID U DO? ✅

**A team task-management web app: assign work, track it, and see who actually did it.**

🌐 **Live:** [dyd.gasco.digital](https://dyd.gasco.digital)

> ### 💡 About this project
> DID U DO? is a **for-fun learning project**. I built it **mostly through vibe coding** (AI-assisted development) to explore how a real web app is made, from the first page to payments, deployment and fixing bugs on a live server.
>
> I did not hand-write most of the code. My goal was to understand how all the pieces of a real product fit together: deciding what to build, testing it, debugging problems with AI help, and running it on my own server. I'm now learning to write this kind of code myself as part of my Software Engineering degree.
>
> *The source code is kept private because it contains server and deployment details. This page describes what the app does and what I learned building it.*

---

## ✨ Features

**Teams and organisations**
- Create an organisation and invite people with a join link
- Roles: promote or demote team members to admin
- Switch between organisations

**Tasks**
- Create tasks, assign them to one or more people, and set due dates
- Checklists, file attachments, comments and emoji reactions on tasks
- Sign off a task when it's done ("Did you do it?")
- Archive old tasks and search through them

**Views**
- Kanban board with drag-and-drop between folders
- Calendar view of due dates
- "My tasks" and "All tasks" lists

**Notifications**
- Email notifications (Resend) and text-message notifications (Twilio)
- Hourly or daily reminders, run on a scheduler

**Team stats**
- Team statistics page (PDF export is planned, not built yet)

**Billing**
- Paystack subscriptions: checkout, webhooks and a billing page

**Other**
- Installable on a phone like an app (PWA: web manifest + service worker)
- Password reset by email
- Custom error pages, including a "too many requests" page

---

## 🛠️ Tech stack

| Area | Tools |
|---|---|
| Backend | Python, Flask, Flask-Login, Flask-APScheduler |
| Database | SQLAlchemy / Flask-SQLAlchemy (SQLite) |
| Frontend | Jinja templates, CSS, JavaScript |
| Integrations | Paystack (payments), Resend (email), Twilio (SMS) |
| Hosting | Ubuntu Linux server, Gunicorn, Nginx, systemd |

---

## 🧠 What I learned

- How a Flask app is structured: routes, templates, models and static files
- How a database is designed with models and relationships, and how to change it safely with migrations
- How to plug in a payment provider and handle webhooks
- How to deploy an app to a Linux server and keep it running as a service
- How to update a live app safely: back up the database first, and never overwrite live data
- How to find and fix real bugs, and how to work with AI tools without blindly trusting them

---

## 🚧 Status

DID U DO? is a personal project and a work in progress. An AI-assisted code review found bugs that I'm still working through, which has been a great way to learn how real software gets maintained.

---

**Built by Jan-Gerhard du Plessis**, Software Engineering student at Eduvos, Pretoria
[LinkedIn](https://www.linkedin.com/in/jan-gerhard-du-plessis-a1814739b/) · [GitHub](https://github.com/JGDP2007)
