# 🔐 Roblox Remote Security Analyzer

A static analysis tool that scans Roblox Lua RemoteEvent and RemoteFunction server code for common security vulnerabilities and unsafe patterns.

---

## 🛡 Purpose

This tool is designed to help Roblox developers strengthen their games by identifying common server-side validation mistakes.

It is strictly:
- ✅ Defensive  
- ✅ Educational  
- ✅ Static analysis only  

It does **not** generate exploits, bypasses, or harmful scripts.

---

## 🚨 What It Detects

- Missing server-side validation  
- Client-trusted value manipulation  
- Direct `leaderstats` modification risks  
- Lack of rate limiting / cooldowns  
- Unsafe input handling  
- Missing type or sanity checks  

---

## 📊 Features

- Security scoring system (0–100)
- Risk classification (Low / Medium / High)
- Clear vulnerability explanations
- Recommended secure coding patterns
- Lightweight and easy to use

---

## 🌐 Live Demo

Try the live analyzer here:

🔗 https://roblox-security-analyzer--programixscript.replit.app/

Also Join The Discord! https://discord.gg/b6njy7yb
---

## 📸 Screenshots

### Example Scan Result
!(screenshots/scan-result.png)

---

## 🧠 Example Issue

```lua
player.leaderstats.Coins.Value = amount
