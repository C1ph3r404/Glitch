# README.md — Glitch (TryHackMe)

**Glitch — TryHackMe WriteUp**

Short: discovered a base64 token at `/api/access` that unlocks the UI, fuzzed `/api/items` to find an `eval`-backed `cmd` parameter, used Node `child_process().exec` to get RCE, harvested Firefox saved passwords to escalate to `v0id`, and used `doas` to read the root flag. Full steps, commands and screenshots in `WriteUp.md`.

## Disclaimer

For labs and learning only. Don’t target systems you don’t own or have permission to test.

---
