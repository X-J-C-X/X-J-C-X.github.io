---
layout: page
title: Home
id: home
permalink: /
tags:
  - internal
  - external
  - index
---

# Welcome! 🌱

<p style="padding: 3em 1em; background: #f5f7ff; border-radius: 4px;">
  Take a look at <span style="font-weight: bold">[[Your first note]]</span> to get started on your exploration.
</p>


<strong>Recently updated notes</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
</style>


# 📧 Knowledge Base Project

## 📚 Main Sections

### [[1-general-kb-index|🔧 1. General Knowledge Base]]

**Authentication**
- [[_notes/1.1-spf|1.1 SPF Records]]
- [[1.2-dkim|1.2 DKIM Signing]]
- [[1.3-dmarc|1.3 DMARC Policy]]

**Encryption**
- [[1.4-smime|1.4 S/MIME]]
- [[1.5-pgp|1.5 PGP/GPG]]
- [[1.6-tls|1.6 TLS/SSL]]

**Protocols**
- [[1.7-smtp|1.7 SMTP]]
- [[1.8-imap|1.8 IMAP]]
- [[1.9-LDAP|1.9 LDAP]]
- [[1.10-mail-headers|1.10 Mail Headers]]

**Platforms**
- [[1.11-m365|1.11 Microsoft 365]]
- [[1.12-exchange|1.12 Exchange Server]]
- [[1.13-outlook|1.13 Outlook Client]]

**DNS**
- [[1.14-mx-records|1.14 MX Records]]
- [[1.15-txt-records|1.15 TXT Records]]
- [[1.16-dns-troubleshooting|1.16 DNS Troubleshooting]]

**Mail Routing**
- [[1.17-mail-routing|1.17 Mail Routing Basics]]
- [[1.18-connectors|1.18 Connectors]]
- [[1.19-mail-flow|1.19 Mail Flow Rules]]

**Troubleshooting**
- [[1.20-delivery-issues|1.20 Delivery Issues]]
- [[1.21-auth-failures|1.21 Authentication Failures]]
- [[1.22-performance|1.22 Performance Issues]]

### [[2-external-index|💬 2. External / Customer Support]]

**Common Issues**
- [[2.1-email-not-received|2.1 Email Not Received]]
- [[2.2-cannot-send|2.2 Cannot Send Email]]
- [[2.3-authentication-error|2.3 Authentication Error]]
- [[2.4-attachment-blocked|2.4 Attachment Blocked]]
- [[2.5-spam|2.5 Email in Spam]]

**How-To Guides**
- [[2.6-setup-email-client|2.6 Setup Email Client]]
- [[2.7-configure-mobile|2.7 Configure Mobile Device]]
- [[2.8-setup-forwarding|2.8 Setup Email Forwarding]]
- [[2.9-create-signature|2.9 Create Email Signature]]

**FAQ**
- [[2.10-password-reset|2.10 Password Reset]]
- [[2.11-storage-quota|2.11 Storage Quota]]
- [[2.12-backup-emails|2.12 Backup Emails]]

### [[3-internal-index|🔒 3. Internal Documentation]]

**Bug Tracking**
- [[3.1-bug-template|3.1 Bug Report Template]]
- [[3.2-known-issues|3.2 Known Issues]]

**Procedures**
- [[3.3-onboarding|3.3 Employee Onboarding]]
- [[3.4-escalation|3.4 Escalation Process]]
- [[3.5-maintenance|3.5 System Maintenance]]
- [[3.6-incident-response|3.6 Incident Response]]

**Incidents**
- [[3.7-incident-template|3.7 Incident Template]]
- [[3.8-postmortem-template|3.8 Postmortem Template]]

---

*Last updated: 2025-01-19*
