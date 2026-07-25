🏥 CareScope Analytics

> A predictive healthcare operations command center that helps hospitals see what is happening now, understand every patient journey, and prepare for what comes next.

CareScope Analytics is a polished, frontend-only Healthcare Analytics SaaS dashboard built for a hackathon qualifier. It transforms complex hospital operations into a calm, actionable workspace for patient flow, resource capacity, clinical activity, scheduling, reporting, and simulated forecasting.

The experience is powered entirely by realistic local mock data. It requires no backend, database, authentication service, or external API.

---

## 💡 Why CareScope?

Hospital teams often work across disconnected tools for appointments, patient records, staffing, beds, diagnostics, and resource planning. That fragmentation makes it difficult to see the full operational picture or respond before capacity becomes critical.

CareScope brings those signals into one responsive command center:

- 👀 **See the present** with live operational metrics and hospital-wide KPIs.
- 🩺 **Understand the patient journey** from admission through discharge.
- 🔮 **Plan ahead** using clearly labelled simulated forecasts.
- 🏨 **Coordinate resources** through capacity monitoring and a Hospital Digital Twin.
- ⚡ **Turn data into action** with scheduling, filtered reporting, and export tools.

---

## 🗺️ Unique Differentiator: Hospital Digital Twin

The **Hospital Digital Twin** is an interactive visual model of the facility. It provides spatial context for departments including:

- OPD
- Radiology
- ICU
- Pharmacy
- Emergency

Selecting a department reveals its operational health, staff availability, patient load, capacity, and recent alerts. This turns a traditional dashboard into an explorable model of the hospital.

---

## ✨ Product Highlights

### 📊 Operations Command Center

- Six animated KPI cards with trend indicators and sparklines
- Patient visits, revenue, disease distribution, bed occupancy, and appointment charts
- Live hospital monitoring with subtly changing metrics
- Responsive sidebar, mobile navigation, live clock, notifications, and profile controls
- Skeleton loading states and smooth entrance animations

### 🔮 Predictive Intelligence

- Simulated patient-load forecast
- Bed-occupancy prediction
- Seasonal disease outlook
- Dashed forecast lines and confidence visualization
- Clear **Forecast — Simulated Data** labels

### 🧑‍⚕️ Patient Care Journey

- Animated vertical treatment timeline
- Admission, diagnostics, diagnosis, treatment, recovery, and discharge states
- PDF-style diagnostic report
- Patient information, laboratory values, physician notes, and print/PDF export

### 📅 Appointment Scheduling

- Interactive week and month calendar views
- Previous, next, and Today navigation
- Department-coded appointments
- In-page booking form for patient, doctor, date, and time selection
- Newly booked appointments appear immediately in the calendar

### 📑 Reports and Exports

- Client-side department and doctor filters
- Live summary calculations
- Detailed clinical activity table
- Real CSV export
- Browser print/PDF support

### 🚑 Resource Management

- ICU beds
- Medical oxygen
- Ventilators
- Blood bank inventory
- Ambulance availability
- Threshold-based utilization indicators
- Doctor availability and workload overview

### 🚀 Productivity Features

- Functional global search across patients, doctors, and reports
- Expandable real-time activity feed
- Blue, emerald, and purple interface presets
- Session-only light and dark themes
- Floating quick actions for appointments, patients, and reports

---

## 🛠️ Technology Stack

| Technology | Purpose |
| --- | --- |
| React 19 | Component-driven user interface |
| TypeScript | Strict typing and safer application logic |
| Vite | Fast development and production builds |
| Tailwind CSS | Utility-first styling foundation |
| Framer Motion | Entrance animations and micro-interactions |
| Recharts | All dashboard and forecast visualizations |
| Lucide React | Consistent icon system |
| React Router | Client-side page navigation |

No UI kit or pre-built dashboard template is used. Components and visual primitives are built specifically for CareScope.

---

## 🧱 Architecture

CareScope is intentionally frontend-only:

```text
src/
├── App.tsx        # Routes, pages, UI components, and interactions
├── data.ts        # Typed, internally consistent hospital mock data
├── main.tsx       # React application entry point
└── styles.css     # Responsive visual system and theme styles
```

All patients, clinicians, appointments, diagnostics, charts, forecasts, and resource values originate from local typed data. No requests are sent to external services.

---

## 🧭 Routes

| Route | Experience |
| --- | --- |
| `/` | Product landing page |
| `/dashboard` | Operational command center and forecasts |
| `/appointments` | Interactive scheduling calendar |
| `/patients` | Patient timeline and diagnostic report |
| `/reports` | Filters, summaries, CSV export, and print view |
| `/resources` | Resource dashboard, doctors, and Digital Twin |
| `/settings` | Appearance presets and hospital profile |

---

## 🚀 Getting Started

### ✅ Requirements

- Node.js 22 or newer
- npm

### 💻 Install and run

```bash
npm install
npm run dev
```

Open the local address shown in the terminal, normally:

```text
http://localhost:5173
```

### 📦 Production build

```bash
npm run build
```

The optimized frontend is generated in the `dist` directory.

---

## ☁️ Deployment

### ▲ Vercel

1. Import the GitHub repository into Vercel.
2. Select **Vite** as the framework preset.
3. Use `npm run build` as the build command.
4. Use `dist` as the output directory.
5. Deploy.

### 🌐 Netlify or other static hosts

Use the same build command and publish the `dist` directory. Configure an SPA fallback to `index.html` so React Router routes work on refresh.

---

## 📱 Responsive Design

The interface is designed and tested around:

- **Mobile:** 375px+
- **Tablet:** 768px+
- **Desktop:** 1280px+

Navigation adapts from a full sidebar to compact and bottom-navigation layouts. Tables, calendars, charts, cards, forms, and the Digital Twin remain accessible on smaller screens.

---

## 🎬 Recommended Demo Flow

For a strong hackathon presentation:

1. Start on the landing page and introduce the operational problem.
2. Launch the dashboard and explain the hospital-wide KPIs.
3. Highlight the simulated forecasts and capacity planning.
4. Book an appointment from the scheduling page.
5. Open the patient journey and diagnostic report.
6. Filter a report and export it as CSV.
7. Finish with the interactive Hospital Digital Twin.

---

## 🛡️ Data and Safety Notice

All people, records, diagnoses, forecasts, laboratory values, and operational metrics are fictional and created solely for demonstration.

CareScope Analytics is not a medical device and must not be used for diagnosis, treatment decisions, or real clinical operations.

---

## 🔭 Future Possibilities

- Secure role-based authentication
- Real hospital information system integrations
- FHIR-compatible clinical data exchange
- Persistent scheduling and report storage
- Alert acknowledgement workflows
- Configurable forecasting models
- Multi-facility comparison

---

## 📜 License

This project was created as a hackathon demonstration. Add a license appropriate to your submission rules before public reuse or distribution.

---

<div align="center">
  <strong>🏥 CareScope Analytics</strong><br />
  Clearer operations. Better preparation. More connected care. 💙
</div>
