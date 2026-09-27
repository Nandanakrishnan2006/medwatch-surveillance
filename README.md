# MedWatch

> A hospital security operations platform for monitoring security events, verifying incidents, and coordinating incident response.

MedWatch is a frontend hackathon prototype designed to demonstrate how intelligent security detection can support hospital security teams while keeping humans responsible for verification and escalation decisions.

The platform combines simulated CCTV monitoring, security alerts, patient location monitoring, human verification, escalation workflows, and audit logging into a single hospital security operations interface.

> **⚠️ Prototype Notice:** MedWatch is a frontend demonstration using mock data. It is not intended for real-world medical, security, or emergency operations.

---

## 📌 Problem Statement

Hospitals are complex environments where security teams need to monitor multiple areas, respond to incidents, and coordinate with clinical staff while protecting patient privacy.

Events such as:

- Patient falls
- Aggressive behavior
- Unexpected patient absence
- Movement outside expected hospital zones
- CCTV failures

can require immediate attention.

However, security teams may face several challenges:

- Monitoring multiple cameras simultaneously
- Identifying important events among routine activity
- Coordinating security and care teams
- Managing false alarms
- Maintaining a clear history of incidents
- Protecting sensitive patient information

Simply generating automated alerts is not enough. Staff need a system that allows them to **review, verify, escalate, and resolve incidents through a clear workflow**.

---

## 💡 Solution

MedWatch provides a centralized hospital security operations interface that helps security personnel monitor events and coordinate responses.

The system uses simulated intelligent detection to identify events such as:

- **Patient Fall**
- **Aggressive Behavior**
- **Unexpected Patient Absence**

When an event is detected, the system creates an alert marked:

> **AI DETECTION — VERIFICATION REQUIRED**

The system does **not automatically escalate** the event.

A security staff member must first review and verify the detection before the incident can move to the next stage.

### Incident Workflow

```text
AI Detection
     ↓
Security Verification
     ↓
Nurse / Care Team Notification
     ↓
Family Notification (if required)
     ↓
Case Resolution
     ↓
Audit Log
