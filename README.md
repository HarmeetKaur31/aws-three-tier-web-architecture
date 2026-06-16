# aws-three-tier-web-architecture

aws-three-tier-web-architecture/
│
├── web-tier/
│   ├── src/
│   ├── public/
│   ├── package.json
│   ├── package-lock.json
│   ├── nginx.conf
│   └── README.md
│
├── app-tier/
│   ├── index.js
│   ├── package.json
│   ├── routes/
│   ├── controllers/
│   ├── models/
│   ├── config/
│   └── README.md
│
├── database/
│   ├── schema.sql
│   ├── seed.sql
│   └── README.md
│
├── infrastructure/
│   ├── architecture-diagram.png
│   ├── aws-setup-notes.md
│   ├── security-groups.md
│   └── load-balancer-config.md
│
├── scripts/
│   ├── deploy-web.sh
│   ├── deploy-app.sh
│   ├── install-nginx.sh
│   └── start-services.sh
│
├── docs/
│   ├── project-setup-guide.md
│   ├── troubleshooting.md
│   └── api-docs.md
│
├── .gitignore
└── README.md
