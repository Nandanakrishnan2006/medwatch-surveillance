# MedWatch Sentinel

## Goal
Build a realistic, interactive hospital security operations prototype at the main app address, using mock data only.

## Experience
- Start with a compact username/password sign-in; any non-empty values open the operations console.
- Use a restrained clinical interface: light surfaces, dark navy text, thin borders, subtle blue/teal status accents, compact spacing, and minimal shadows.
- Provide a persistent left navigation and top operational status bar, with a mobile-friendly navigation treatment.

## Screens and interactions
- **Overview:** camera, alert, patient, and zone totals plus a chronological live event feed.
- **Live Surveillance:** realistic simulated corridor/common-area camera panels, health/timestamp labels, and controls for fall, aggressive behavior, and patient-leaving events.
- **Security Alerts:** searchable/filterable alert queue and a detail view with event facts, required human verification, camera access, and the full escalation path.
- **Patient Monitoring:** privacy-conscious patient IDs, expected/current zones, last-seen times, and absence warnings only.
- **Hospital Zones:** operational zone status and coverage summaries.
- **CCTV Health:** camera connectivity and system checks.
- **Audit Log:** realistic timestamped actions and status changes.
- **Security Controls:** restrained indicators for role access, session, permission checks, audit logging, privacy constraints, and prototype limitations.

## Workflow behavior
- Simulations create alerts, update overview counts and event history, and append audit entries.
- New detections remain at “AI DETECTION — VERIFICATION REQUIRED” until a security operator verifies or rejects them.
- Verified alerts can progress through care-team notification, optional family notification, case resolution, and final audit logging.
- Rejected alerts become false alarms and are recorded without escalation.
- Patient-leaving simulations update the corresponding patient’s last-known location and warning status.

## Technical details
- Keep all state in the browser for this frontend prototype; no real login or patient data is used.
- Use TanStack Router’s existing main route, React state, semantic design tokens, and accessible controls.
- Add route-specific page metadata and verify core flows at desktop and mobile widths.
