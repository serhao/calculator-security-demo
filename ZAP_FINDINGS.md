# ZAP Findings Table

| Code | Issue | Risk | Affected | Why It Matters |
|------|-------|------|----------|----------------|
| 10038 | Content Security Policy (CSP) Header Not Set | Medium | http://localhost:5000 | Prevents XSS and data injection attacks |
| 10020 | Missing Anti-clickjacking Header | Medium | http://localhost:5000 | Prevents clickjacking attacks |
| 10106 | HTTP Only Site | Medium | http://localhost:5000 | Data transmitted unencrypted, vulnerable to interception |
| 90004 | Insufficient Site Isolation Against Spectre | Low | http://localhost:5000 | Missing Cross-Origin headers for Spectre protection |
| 10063 | Permissions Policy Header Not Set | Low | http://localhost:5000 | Doesn't restrict browser features (camera, mic, etc.) |
| 10036 | Server Leaks Version Information | Low | http://localhost:5000 | Reveals "Werkzeug/2.0.1 Python/3.9.25" |
| 10021 | X-Content-Type-Options Header Missing | Low | http://localhost:5000 | Allows MIME-sniffing attacks |
