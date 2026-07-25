# CareScope Analytics

CareScope Analytics is a frontend-only healthcare operations SaaS experience created for a hackathon qualifier. It gives hospital leadership a calm, real-time command center for patient flow, capacity, clinical activity, forecasts, and resource planning.

## Highlights

- Operations dashboard with six KPIs, five Recharts visualizations, live monitoring, scheduling, and simulated predictive intelligence
- Patient detail experience with an animated treatment timeline and PDF-style diagnostic report
- Week/month appointment scheduling with department and status coding
- Custom reports with client-side filtering and real CSV export
- Resource command center for ICU beds, oxygen, ventilators, blood bank, and ambulances
- Doctor availability and workload cards
- Responsive navigation optimized for 375px, 768px, and 1280px+ screens
- Session-only light/dark theme through React context
- Skeleton loading, entrance motion, notifications, profile menu, and live clock
- Functional global search across patients, doctors, and reports
- Expandable real-time activity feed for clinical and operational events
- Blue, emerald, and purple session-only theme color presets
- Floating quick actions for appointments, patients, and reports

## Unique differentiator: Hospital Digital Twin

The Hospital Digital Twin presents the facility as a simplified interactive live map. Teams can select OPD, Radiology, ICU, Pharmacy, or Emergency to see capacity, staffing, patient load, operational state, and recent alerts in context.

## Architecture

The app uses React 19, strict TypeScript, Vite, Tailwind CSS, Framer Motion, Recharts, Lucide React, and React Router. All clinical and operational information lives in a single typed local mock-data module. There is no backend, database, persistence layer, external API, or UI component library.

## Local development

```bash
npm install
npm run dev
```

Create a production build with `npm run build`.

> All people, records, forecasts, and clinical values shown are fictional and for demonstration only.
