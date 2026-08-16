# 🔗 Lab 04 — Alert Correlation & Timeline

## 🎯 Objective

Practice correlating multiple security events into a single investigation timeline from a SOC Analyst L1 perspective.

> This is a simulated educational scenario and does not represent a real security incident.

## 🚨 Scenario

A workstation generates multiple security alerts within a related time period:

1. Multiple failed authentication attempts
2. A successful authentication event
3. Unexpected outbound network activity

The objective is to determine whether these events are related and what additional evidence should be collected.

## 📊 Simulated Event Timeline

| Time | Event                                   | Initial Assessment     |
| ---- | --------------------------------------- | ---------------------- |
| T1   | Multiple failed authentication attempts | Requires review        |
| T2   | Successful authentication               | Requires correlation   |
| T3   | Unexpected outbound connection          | Requires investigation |

> The timeline above is a simulated investigation framework, not real event data.

## 🔎 Correlation Questions

The analyst should determine:

* Are all events associated with the same user?
* Are they associated with the same host?
* Did the successful login occur shortly after the failed attempts?
* Is the source of the authentication activity expected?
* Which process initiated the outbound connection?
* Did the network activity occur after the authentication event?
* Are there additional alerts around the same timeframe?

## 🧠 Investigation Methodology

```text
Authentication Failures
        ↓
Successful Authentication
        ↓
Identify User & Host
        ↓
Review Process Activity
        ↓
Review Network Activity
        ↓
Build Timeline
        ↓
Correlate Evidence
        ↓
Assess Risk
        ↓
Escalate if Required
```

## 🚦 Triage Assessment

**Initial Status:** Requires investigation.

**Initial Severity:** Medium.

The final severity should be determined only after reviewing the supporting evidence and environmental context.

## 📝 Analyst Notes

### Timeline

**T1:** Multiple failed authentication events — evidence required.

**T2:** Successful authentication — correlate with previous failures.

**T3:** Outbound network activity — identify process and destination.

### Key Questions

* What account was involved?
* What host was involved?
* What was the source of the authentication attempts?
* Was the successful login expected?
* What process generated the network connection?
* Are the events temporally related?

## 🛡️ Recommended L1 Actions

1. Validate each alert.
2. Preserve relevant evidence.
3. Establish a complete timeline.
4. Correlate user, host, process, and network information.
5. Check for additional related alerts.
6. Document the investigation.
7. Escalate according to the organization's incident-response procedure if suspicious activity is confirmed.

## 🎓 Skills Demonstrated

* SIEM alert correlation
* Timeline analysis
* Authentication investigation
* Network-event correlation
* Evidence collection
* SOC Analyst L1 triage
* Incident documentation
* Escalation methodology

## ⚠️ Disclaimer

This is a simulated cybersecurity lab created for educational and portfolio purposes. It does not represent a real-world security incident.
