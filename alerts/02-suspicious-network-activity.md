# 🌐 Lab 02 — Suspicious Network Activity Alert

## 🎯 Objective

Practice investigating a simulated SIEM alert involving unexpected network activity from a workstation.

> This is an educational simulation and does not represent a real security incident.

## 🚨 Alert Scenario

A SIEM detects an unexpected outbound connection from a workstation to an external destination.

### Alert Details

| Field       | Value                                  |
| ----------- | -------------------------------------- |
| Alert Type  | Unexpected Outbound Network Connection |
| Severity    | Medium                                 |
| Status      | Open                                   |
| Host        | `LAB-WORKSTATION`                      |
| Source      | Simulated                              |
| Destination | `SIMULATED-EXTERNAL-ENDPOINT`          |
| Environment | Authorized Lab                         |

## 🔎 Initial Triage

The L1 analyst should determine:

* Which host generated the connection?
* Which process initiated it?
* What destination was contacted?
* Which port and protocol were used?
* When did the connection occur?
* Is the destination expected?
* Is the process associated with a known application?

## 📊 Evidence to Collect

Relevant evidence may include:

* Timestamp
* Source host
* Source IP
* Destination IP or hostname
* Destination port
* Protocol
* Process name
* User account
* Related security events

## 🧠 Analyst Reasoning

An unexpected outbound connection is **not automatically malicious**.

Possible explanations include:

* Normal application traffic
* Software updates
* Browser activity
* System services
* Misconfigured applications
* Potentially suspicious activity

The analyst should establish context before assigning a higher severity.

## 🔗 Correlation

The network alert should be correlated with other available events:

```text
Network Alert
      ↓
Identify Process
      ↓
Identify User
      ↓
Review Authentication Events
      ↓
Review Process Activity
      ↓
Check Timeline
      ↓
Assess Risk
```

## 🚦 Triage Decision

**Initial Severity:** Medium

**Current Assessment:** Requires investigation.

### Recommended Next Steps

1. Validate the network event.
2. Identify the process responsible.
3. Identify the associated user.
4. Review the destination and port.
5. Check for related authentication events.
6. Check for unusual process activity.
7. Determine whether the connection is expected.
8. Escalate if multiple suspicious indicators are correlated.

## 📝 Analyst Notes

**Finding:** Pending evidence review.

**Confidence:** Low until supporting evidence is collected.

**Escalation:** Not determined at initial triage.

## 🎓 Skills Demonstrated

* SIEM alert triage
* Network activity analysis
* Process correlation
* Event correlation
* Timeline development
* SOC L1 investigation methodology

## ⚠️ Disclaimer

This is a simulated cybersecurity lab created for educational and portfolio purposes. It does not represent a real-world security incident.
