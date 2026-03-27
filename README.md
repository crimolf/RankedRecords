# RankedRecords 🏋️

**Social performance tracking platform for fitness enthusiasts.**  
Track your progress, share achievements, and compete with the community.

🔗 **Live at [rankedrecords.com](https://rankedrecords.com)**

---

## 📸 Screenshots

<!-- Replace with your actual screenshots -->
<p align="center">
  <img alt="home" src="https://github.com/user-attachments/assets/99ba64cc-5fbc-44b3-b5a1-4f2efdbf15ab" width="400"/>
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

### Frontend
| Tech | Role |
|---|---|
| Next.js | Framework (SSR, routing) |
| React | UI components |
| TypeScript | Type safety |
| Tailwind CSS | Styling |
| HeroUI | Component library |

### Backend
| Tech | Role |
|---|---|
| Java 17 | Language |
| Spring Boot | Application framework |
| Spring Security | Authentication (JWT) |
| JPA / Hibernate | ORM |
| PostgreSQL | Database |

### Infrastructure
| Tech | Role |
|---|---|
| Docker | Containerization |
| Google Cloud Run | Backend hosting |
| Vercel | Frontend hosting |
| AWS S3 | Image storage |
| Cloudflare | DNS & security |

---

## 🏗️ Architecture

```
┌─────────────────┐        ┌──────────────────┐
│   Next.js App   │  HTTP  │  Spring Boot API  │
│   (Vercel)      │◄──────►│  (Cloud Run)      │
└─────────────────┘        └────────┬─────────┘
                                    │
                    ┌───────────────┼───────────────┐
                    │               │               │
             ┌──────▼─────┐  ┌─────▼──────┐  ┌────▼────┐
             │ PostgreSQL  │  │   AWS S3   │  │Cloudflare│
             │ (Database)  │  │  (Images)  │  │  (DNS)  │
             └────────────┘  └────────────┘  └─────────┘
```

The frontend is fully decoupled from the backend and communicates via REST API.  
The backend handles authentication, business logic, and data persistence.  
Images are stored on AWS S3 and served directly to the client.

---

## 📁 Related

> The source code for this project is kept private.  
> Feel free to reach out on [LinkedIn](https://linkedin.com/in/alessandro-lupo) if you want to know more.
