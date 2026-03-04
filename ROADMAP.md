# ServerKit Roadmap

This document outlines the development roadmap for ServerKit. Features are organized by phases and priority.

---

## Current Version: v0.9.0

### Recently Completed

- **Two-Factor Authentication (2FA)** - TOTP-based with backup codes
- **Notification Webhooks** - Discord, Slack, Telegram, generic webhooks
- **ClamAV Integration** - Malware scanning with quarantine
- **File Integrity Monitoring** - Baseline creation and change detection
- **Environment Variable Management** - Secure, encrypted per-app variables
- **Cron Job Management** - Visual cron editor
- **Server Uptime Tracking** - Historical uptime data and visualization

---

## Phase 1: Core Infrastructure (Completed)

- [x] Flask backend with SQLAlchemy ORM
- [x] React frontend with Vite
- [x] JWT-based authentication
- [x] Real-time WebSocket updates
- [x] System metrics (CPU, RAM, disk, network)
- [x] Docker and Docker Compose support
- [x] SQLite/PostgreSQL database support

---

## Phase 2: Application Management (Completed)

- [x] PHP/WordPress application deployment
- [x] Python (Flask/Django) application support
- [x] Node.js application management with PM2
- [x] Docker container management
- [x] Environment variable management
- [x] Application start/stop/restart controls
- [x] Log viewing per application

---

## Phase 3: Domain & SSL Management (Completed)

- [x] Nginx virtual host management
- [x] Domain configuration interface
- [x] Let's Encrypt SSL integration
- [x] SSL certificate auto-renewal
- [x] Redirect management (HTTP → HTTPS)

---

## Phase 4: Database Management (Completed)

- [x] MySQL/MariaDB database support
- [x] PostgreSQL database support
- [x] Database creation/deletion
- [x] User management per database
- [x] Basic query interface

---

## Phase 5: File & FTP Management (Completed)

- [x] Web-based file manager
- [x] File upload/download
- [x] File editing with syntax highlighting
- [x] vsftpd FTP server integration
- [x] FTP user management

---

## Phase 6: Monitoring & Alerts (Completed)

- [x] Real-time system metrics
- [x] Server uptime tracking
- [x] Customizable alert thresholds
- [x] Discord webhook notifications
- [x] Slack webhook notifications
- [x] Telegram bot notifications
- [x] Generic webhook support
- [x] Alert history and logging

---

## Phase 7: Security Features (Completed)

- [x] Two-factor authentication (TOTP)
- [x] Backup codes for 2FA recovery
- [x] ClamAV malware scanning
- [x] Quick scan / Full scan options
- [x] File quarantine management
- [x] File integrity monitoring
- [x] Failed login detection
- [x] Security event logging

---

## Phase 8: Scheduled Tasks (Completed)

- [x] Cron job management
- [x] Visual cron expression builder
- [x] Job execution history
- [x] Enable/disable jobs

---

## Phase 9: Firewall Management (Completed - Merged into Security)

- [x] UFW firewall integration
- [x] Visual rule management
- [x] Common port presets
- [x] Rule enable/disable
- [x] Consolidated into Security page for unified security management

---

## Phase 10: Multi-Server Management (In Progress)

**Priority: High**

- [x] Agent-based remote server monitoring (Go agent)
- [x] Centralized dashboard for multiple servers
- [x] Server grouping and tagging
- [x] Cross-server metrics comparison
- [x] Remote Docker management via agents
- [x] Server health overview
- [x] Agent WebSocket gateway
- [x] HMAC-SHA256 authentication
- [x] GitHub Actions for agent releases (Linux/Windows)
- [x] Installation scripts endpoint
- [x] Agent auto-update mechanism
- [x] Agent download page in UI
- [x] Container logs streaming for remote servers

---

## Phase 11: Git Deployment (Planned)

**Priority: High**

- [x] GitHub/GitLab webhook integration
- [x] Automatic deployment on push
- [x] Branch selection for deployment
- [x] Rollback to previous deployments
- [x] Deployment history and logs
- [x] Pre/post deployment scripts
- [x] Zero-downtime deployments

---

## Phase 12: Backup & Restore (Completed)

**Priority: High**

- [x] Automated database backups
- [x] File/directory backups
- [x] S3-compatible storage support
- [x] Backblaze B2 integration
- [x] Backup scheduling
- [x] One-click restore
- [x] Backup retention policies
- [x] Offsite backup verification

---

## Phase 13: Email Server Management (Completed)

**Priority: Medium**

- [x] Postfix mail server setup
- [x] Dovecot IMAP/POP3 configuration
- [x] Email account management
- [x] Spam filtering (SpamAssassin)
- [x] DKIM/SPF/DMARC configuration
- [x] Webmail interface integration
- [x] Email forwarding rules

---

## Phase 14: Advanced SSL Features (Planned)

**Priority: Medium**

- [ ] Wildcard SSL certificates
- [ ] Multi-domain certificates (SAN)
- [ ] Custom certificate upload
- [ ] Certificate expiry monitoring
- [ ] Automatic renewal notifications

---

## Phase 15: Team & Permissions (Planned)

**Priority: Medium**

- [ ] Multi-user support
- [ ] Role-based access control (RBAC)
- [ ] Custom permission sets
- [ ] Audit logging per user
- [ ] Team invitations
- [ ] Activity dashboard

---

## Phase 16: API Enhancements (Planned)

**Priority: Medium**

- [ ] API key management
- [ ] Rate limiting
- [ ] Webhook event subscriptions
- [ ] OpenAPI/Swagger documentation
- [ ] API usage analytics

---

## Phase 17: Advanced Security (Completed)

**Priority: High**

- [x] Unified Security page with all security features
- [x] Firewall tab with UFW/firewalld management
- [x] Fail2ban integration
- [x] SSH key management
- [x] IP allowlist/blocklist
- [x] Brute force protection
- [x] Security audit reports
- [x] Vulnerability scanning (Lynis)
- [x] Automatic security updates (unattended-upgrades/dnf-automatic)

---

## Phase 18: Performance Optimization (Planned)

**Priority: Low**

- [ ] Redis caching integration
- [ ] Database query optimization
- [ ] Static asset CDN support
- [ ] Lazy loading for large datasets
- [ ] Background job queue (Celery)

---

## Phase 19: Mobile App (Planned)

**Priority: Low**

- [ ] React Native mobile application
- [ ] Push notifications
- [ ] Quick actions (restart, view stats)
- [ ] Biometric authentication

---

## Phase 20: Marketplace & Extensions (Planned)

**Priority: Low**

- [ ] Plugin/extension system
- [ ] Community marketplace
- [ ] Custom dashboard widgets
- [ ] Theme customization

---

## Phase 21: SSO & OAuth Login (Completed)

**Priority: High**

- [x] Google OAuth 2.0 login
- [x] GitHub OAuth login
- [x] Generic OpenID Connect (OIDC) provider support
- [x] SAML 2.0 support for enterprise environments
- [x] Social login UI (provider buttons on login page)
- [x] Account linking (connect OAuth identity to existing local account)
- [x] Auto-provisioning of new users on first SSO login
- [x] Configurable SSO settings (enable/disable providers, client ID/secret management)
- [x] Enforce SSO-only login (disable password auth for team members)
- [x] SSO session management and token refresh

---

## Phase 22: Database Migrations & Schema Versioning (Planned)

**Priority: High**

Matomo-style update wizard — when the user logs in after an update and there are pending migrations, a popup/wizard guides them through the process visually.

### Backend — Migration Engine
- [ ] Integrate Flask-Migrate (Alembic) for versioned schema migrations
- [ ] Generate initial migration from current model state as baseline
- [ ] Replace `_auto_migrate_columns()` hack with proper Alembic migrations
- [ ] Store schema version in a `schema_version` table (current version, history)
- [ ] API endpoint to check migration status (`GET /api/v1/system/migrations`)
- [ ] API endpoint to run pending migrations (`POST /api/v1/system/migrations/apply`)
- [ ] API endpoint to rollback last migration (`POST /api/v1/system/migrations/rollback`)
- [ ] Auto-detect pending migrations on login and flag the session
- [ ] Pre-migration automatic DB backup before applying changes
- [ ] Migration scripts for all existing model changes (retroactive baseline)

### Frontend — Update Wizard UI
- [ ] Full-screen modal/wizard that appears when pending migrations are detected
- [ ] Step 1: "Update Available" — show current version vs new version, changelog summary
- [ ] Step 2: "Backup" — auto-backup the database, show progress, confirm success
- [ ] Step 3: "Apply Migrations" — run migrations with real-time progress/log output
- [ ] Step 4: "Done" — success confirmation with summary of changes applied
- [ ] Error handling: if a migration fails, show the error and offer rollback option
- [ ] Block access to the panel until migrations are applied (like Matomo does)
- [ ] Migration history page in Settings showing all past migrations and timestamps

### CLI Fallback
- [ ] CLI commands for headless/SSH scenarios (`flask db upgrade`, `flask db status`)
- [ ] CLI rollback support (`flask db downgrade`)

---

## Version Milestones

| Version | Target Features | Status |
|---------|-----------------|--------|
| v0.9.0 | Core features, 2FA, Notifications, Security | Current |
| v1.0.0 | Production-ready stable release, DB migrations | Planned |
| v1.1.0 | Multi-server, Git deployment | Planned |
| v1.2.0 | Backups, Advanced SSL, Advanced Security | Planned |
| v1.3.0 | Email server, API enhancements | Planned |
| v1.4.0 | Team & permissions, SSO & OAuth login | Planned |
| v1.5.0 | Performance optimizations | Planned |
| v2.0.0 | Mobile app, Marketplace | Future |

---

## Contributing

Want to help? See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

**Priority areas for contributions:**
- Multi-server agent development
- Git webhook integration
- S3/B2 backup implementations
- Additional notification channels
- UI/UX improvements
- Documentation

---

## Feature Requests

Have a feature idea? Open an issue on GitHub with the `enhancement` label.

---

<p align="center">
  <strong>ServerKit Roadmap</strong><br>
  Last updated: March 2026
</p>
