# Developer Commands Cheat Sheet

A simple reference for commonly used to generate secret keys.

---

## Secret Key Generation Commands


```bash
# Using OpenSSL
openssl rand -hex 64

# Using Node.js directly in terminal
node -e "console.log(require('crypto').randomBytes(64).toString('hex'))"

# Using Linux / macOS built-in head and base64
head -c 64 /dev/urandom | base64

```
