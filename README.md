# basket-case
Jira alternative

'''
  jira-lite/
  ├─ .github/
  │   └─ workflows/
  │       └─ ci.yml               # GitHub Actions CI pipeline
  ├─ backend/
  │   ├─ cmd/
  │   │   └─ server/              # main.go (entry point)
  │   ├─ internal/
  │   │   ├─ db/                  # DB models & migrations (sqlc or gorm)
  │   │   ├─ api/                 # HTTP handlers (Gin routes)
  │   │   ├─ auth/                # GitHub OAuth helper
  │   │   └─ service/             # Business logic (issue service, workflow)
  │   ├─ go.mod
  │   └─ Dockerfile               # multi‑stage build
  ├─ frontend/
  │   ├─ src/
  │   │   ├─ components/
  │   │   │   ├─ Board.tsx        # Kanban board with drag‑and‑drop
  │   │   │   ├─ IssueForm.tsx
  │   │   │   └─ IssueCard.tsx
  │   │   ├─ pages/
  │   │   │   └─ ProjectView.tsx
  │   │   ├─ api/                 # thin wrapper around backend REST
  │   │   └─ App.tsx
  │   ├─ package.json
  │   ├─ tsconfig.json
  │   └─ Dockerfile               # build static assets, serve via nginx
  ├─ docs/
  │   ├─ openapi.yaml             # OpenAPI spec
  │   └─ mkdocs.yml
  ├─ scripts/
  │   └─ migrate.sh               # run DB migrations locally
  └─ README.md
'''
