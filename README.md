# 🌐 Web Attack Detection in SIEM

## 🧭 Project Summary

This detection engineering lab focuses on identifying common web application attacks such as SQL injection, XSS, and path traversal.

---

## 🎯 Objectives

* Simulate web attacks
* Analyze web logs
* Build SIEM detections
* Detect encoded payloads

---

## ⚔️ Attack Simulation

Payloads included in:

```
attacks/web_attack_payloads.txt
```

---

## 🔍 Detection Strategy

### Indicators

* SQL keywords
* Script tags
* Encoded payloads
* Error spikes

### Example SPL

```spl
index=web_logs
| search "UNION SELECT" OR "<script>" OR "../"
```

---

## 🚨 MITRE ATT&CK

* T1190
* T1059

---

## 📊 Expected Findings

* Injection attempts
* XSS probes
* Directory traversal

---

## 🔮 Future Improvements

* WAF integration
* Regex tuning
* ML anomaly detection

---

## ⚠️ Disclaimer

Educational use only.
