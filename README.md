# RankedRecords 🏋️

**Social performance tracking platform for fitness enthusiasts.**  
Track your progress, share achievements, and compete with the community.

🔗 **Live at [rankedrecords.com](https://rankedrecords.com)**

---

## 📸 Screenshots

<!-- Replace with your actual screenshots -->
<p align="center">
  <img alt="home" src="https://github.com/user-attachments/assets/c07ee680-a5b0-4273-9683-90d4181a910a" width="400"/>
  <img alt="stats" src="https://github.com/user-attachments/assets/7682e681-c0a3-414e-8b88-65ee8e24f6cb" width="400"/>
</p>

<p align="center">
  <img alt="feed" src="https://github.com/user-attachments/assets/6e683e85-ceeb-4c3e-887e-e4856cd00fb1" width="260"/>
  <img alt="search" src="https://github.com/user-attachments/assets/d2e8eccf-aea0-48b6-8019-30bb5e4b09d1" width="260"/>
  <img alt="profile" src="https://github.com/user-attachments/assets/f1a67623-8c47-4dab-afa4-e295f28cd0ba" width="260"/>
</p>






---

## ✨ Features

- **Performance tracking** — log and monitor your fitness progress over time
- **Social feed** — share achievements and engage with the community
- **Rankings** — compete and compare with other users
- **Profile & stats** — personal dashboard with history and metrics
- **Image uploads** — attach photos to your posts and profile
- **Authentication** — secure JWT-based login system

---


## 🔧 Tech Stack

<table>
  <tr>
    <th>Frontend</th>
    <th>Backend</th>
    <th>Infrastructure</th>
  </tr>
  <tr>
    <td valign="top">
      <b>Next.js</b> — Framework (SSR, routing)<br/>
      <b>React</b> — UI components<br/>
      <b>TypeScript</b> — Type safety<br/>
      <b>Tailwind CSS</b> — Styling<br/>
      <b>HeroUI</b> — Component library
    </td>
    <td valign="top">
      <b>Java 17</b> — Language<br/>
      <b>Spring Boot</b> — Application framework<br/>
      <b>Spring Security</b> — Authentication (JWT)<br/>
      <b>JPA / Hibernate</b> — ORM<br/>
      <b>PostgreSQL</b> — Database
    </td>
    <td valign="top">
      <b>Docker</b> — Containerization<br/>
      <b>Google Cloud Run</b> — Backend hosting<br/>
      <b>Vercel</b> — Frontend hosting<br/>
      <b>AWS S3</b> — Image storage<br/>
      <b>Cloudflare</b> — DNS & security
</td>
  </tr>
</table>

---

## 🏗️ Architecture

```
┌─────────────────┐        ┌──────────────────┐
│   Next.js App   │  HTTP  │  Spring Boot API │
│   (Vercel)      │◄──────►│  (Cloud Run)     │
└─────────────────┘        └────────┬─────────┘
                                    │
                    ┌───────────────┼───────────────┐
                    │               │               │
             ┌──────▼─────┐  ┌─────▼──────┐  ┌────▼─────┐
             │ PostgreSQL │  │   AWS S3   │  │Cloudflare│
             │ (Database) │  │  (Images)  │  │  (DNS)   │
             └────────────┘  └────────────┘  └──────────┘
```

The frontend is fully decoupled from the backend and communicates via REST API.  
The backend handles authentication, business logic, and data persistence.  
Images are stored on AWS S3 and served directly to the client.

---
> The source code for this project is kept private.  
> Feel free to reach out on [LinkedIn](https://linkedin.com/in/alessandro-lupo) if you want to know more.
