# GateKeeper

## Specification Deliverable

### Elevator pitch

GateKeeper, the ultimate logbook replacement for security teams! Designed to make logging incidents easier and more
accurate, GateKeeper allows guards to quickly record and track events in real-time. No more messy paperwork or 
hard-to-read entries — this app streamlines the process with powerful search and filtering features, so finding
logs by category or keyword is faster than ever. Plus, with live data updates, your entire team stays in sync,
receiving the latest information on the go, ensuring that everyone is always up to date.

### Design

![Mock](images/mock.jpg)

### Key features

- Secure login to account and to logbooks (companies would have different logbooks)
- Tailored for security guards, law and parking enforcement officers, custodians, building and facility managers, and more.
- Ability to enter logs for any kind of need, whether it is for patrols, simple and complex bookkeeping tasks, incident reporting, equipment checks, maintenance requests, or any other operational activity.
- Logs, users, and logbooks are persistently stored.
- Log templates with required and optional fields, lists, and event categories, make the logging process faster and more accurate.
- Advanced filters and search bars eliminate the need to sift through endless pages of physical logbooks.

### Technologies

I am going to use the required technologies in the following ways.


[TODO 👇]
- **HTML** - Uses correct HTML structure for application. Two HTML pages. One for login and one for voting. Hyperlinks to choice artifact.
- **CSS** - Application styling that looks good on different screen sizes, uses good whitespace, color choice and contrast.
- **React** - Provides login, choice display, applying votes, display other users votes, and use of React for routing and components.
- **Service** - Backend service with endpoints for:
    - login
    - retrieving choices
    - submitting votes
    - retrieving vote status
- **DB/Login** - Store users, choices, and votes in database. Register and login users. Credentials securely stored in database. Can't vote unless authenticated.
- **WebSocket** - As each user votes, their votes are broadcast to all other users.