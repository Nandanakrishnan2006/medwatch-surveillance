# Sentinel Watch

Build a realistic hospital security operations web app called “MedWatch Sentinel”. Make it interactive.

IMPORTANT DESIGN DIRECTION:
Do NOT make this look like an AI-generated SaaS landing page or futuristic AI dashboard.
It should look like a real internal hospital security product that could be used by trained staff.

DESIGN:
- Clean enterprise hospital/SOC interface
- White and very light gray background
- Dark navy typography
- Subtle blue and teal accents
- Thin borders
- Small, restrained status badges
- Compact cards
- Consistent spacing and alignment
- Minimal shadows
- No gradients
- No glowing effects
- No oversized headings
- No unnecessary illustrations
- No AI brain/robot graphics
- No excessive rounded-pill UI
- Avoid the typical “AI startup” aesthetic

The interface should feel functional, serious, trustworthy and slightly clinical.

LOGIN:
Create a simple dummy login screen.
Username + password.
Any non-empty values allow login.
No real authentication yet.

MAIN APPLICATION:

Left sidebar:
- Overview
- Live Surveillance
- Security Alerts
- Patient Monitoring
- Hospital Zones
- CCTV Health
- Audit Log
- Security Controls

Top bar:
- Hospital / MedWatch Sentinel
- Current user role
- System status
- Session status

OVERVIEW:
Show a concise operations dashboard:
- Cameras Online
- Active Alerts
- Patients Monitored
- Zones Monitored

Below that, show:
LIVE SECURITY EVENTS
A chronological list of recent events.

LIVE SURVEILLANCE:
Show realistic CCTV panels representing hospital corridors and common areas.

Each camera panel should contain:
- Camera ID
- Hospital zone
- Online/offline status
- Timestamp
- Simulated video feed

Provide small demo controls:
- Simulate Fall
- Simulate Aggressive Behavior
- Simulate Patient Leaving

DETECTION:
The system can detect:
- Patient Fall
- Aggressive Behavior
- Unexpected Patient Absence

When triggered, create a security alert.

Alert must clearly show:
EVENT
CAMERA / ZONE
TIME
SEVERITY
PATIENT ID if applicable

Use wording:
“AI DETECTION — VERIFICATION REQUIRED”

Do not automatically escalate the event.

ESCALATION WORKFLOW:

AI Detection
→ Security Verification
→ Nurse / Care Team Notification
→ Family Notification if required
→ Case Resolution
→ Audit Log

Make this workflow visually obvious in the alert detail page.

HUMAN VERIFICATION:
Security personnel must have:
- Verify
- Reject / False Alarm
- View Camera

Only after verification can the event move to the next escalation level.

PATIENT MONITORING:
Show privacy-conscious information only:
- Patient ID
- Expected Zone
- Current/Last Detected Zone
- Last Seen
- Status

Do NOT display patient names, diagnoses, medications or unnecessary medical information.

For missing-patient detection, show:
“Unexpected absence detected”
“Last seen: Corridor A”
“Staff verification required”

AUDIT LOG:
Create a realistic table:
Timestamp | Event | User | Action | Status

Examples:
Security verified alert
Nurse notified
Family notification initiated
Case resolved
False alarm recorded

CYBERSECURITY:
Include subtle indicators for:
- Role-based access
- Session status
- Permission checks
- CCTV health
- Audit logging

PRIVACY:
Represent cameras only in appropriate hospital common/security areas.
No cameras in bathrooms, changing rooms or other private spaces.
No facial recognition in this prototype.

FUNCTIONALITY:
This is a frontend hackathon prototype.
Use mock data.
Make the simulated events actually update the dashboard, alerts and audit log.
Make it interactive.

Keep the UI restrained and believable.
Prioritize usability and workflow clarity over visual effects.

This project was built with [Lovable](https://lovable.dev).

**Live app**: https://medwatch-surveillance.lovable.app

## Build with Lovable

Continue developing this project in the [Lovable editor](https://lovable.dev/projects/924c7709-e283-41d0-b43c-50eb020948fd).

- **Ship faster**: describe what you want to build and Lovable handles the code.
- **Stay in sync**: every change made in Lovable is committed straight to this repository.
- **Full ownership**: this code is yours. Push to `main` on GitHub and your changes sync back into Lovable, ready for your next prompt.

## Development

Prefer working locally? You need Node.js and npm — [install with nvm](https://github.com/nvm-sh/nvm#installing-and-updating).

```sh
git clone <this-repository-url>
cd <repository-name>
npm i
npm run dev
```
