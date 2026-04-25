# Security Policy

## Supported Versions

| Version | Supported |
|---------|-----------|
| v2.0.x  | ✅ Active support |
| v1.2.x  | ⚠️ Critical fixes only |
| < v1.2  | ❌ No longer supported |

---

## Security Features

| Feature | Protection |
|---------|------------|
| **SQLCipher** | AES-256 encrypted local database |
| **Hardware Lock** | License bound to machine UUID |
| **Supabase RLS** | Row-level security policies |
| **Device Registry** | Server-controlled device management |
| **Audit Trail** | 90-day action logging |
| **Role-Based Access** | Principal, Admin, Staff permissions |

---

## Reporting a Vulnerability

StuSync handles sensitive student and institutional data. **Do not open public issues** for security vulnerabilities.

**Report privately to:**
- 📧 **Email:** trehiveofficial@gmail.com
- 📝 **Subject:** `[SECURITY] Brief description`

**Response times:**
- Acknowledge: within 48 hours
- Fix: within 14 days (depending on severity)

---

## Scope

- Authentication and license validation bypass
- Unauthorized access to student or financial data
- Database encryption weaknesses
- Sync/cloud data exposure vulnerabilities

---

*© 2024–2026 Trehive*