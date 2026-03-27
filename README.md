# RankedRecords 🏋️

**Social performance tracking platform for fitness enthusiasts.**  
Track your progress, share achievements, and compete with the community.

🔗 **Live at [rankedrecords.com](https://rankedrecords.com)**

---

## 📸 Screenshots

<!-- Replace with your actual screenshots -->
![RankedRecords Demo](./screenshots/demo.gif)

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
