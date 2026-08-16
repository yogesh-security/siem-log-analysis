# 🔐 Lab 03 — Multiple Failed Login Investigation

## 🎯 Objective

Practice investigating repeated failed authentication attempts and determine how an L1 SOC analyst should triage, document, and escalate the activity.

> This is a simulated educational scenario and does not represent a real security incident.

## 🚨 Alert Scenario

The SIEM detects multiple failed authentication attempts against a user account within a defined time window.

### Alert Details

| Field       | Value                  |
| ----------- | ---------------------- |
| Alert Type  | Multiple Failed Logins |
| Severity    | Medium                 |
| Status      | Open                   |
| User        | `lab-user`             |
| Host        | `LAB-WORKSTATION`      |
| Source      | Simulated              |
| Environment | Authorized Lab         |

## 🔎 Investigation Questions

The analyst should determine:

1. How many authentication failures occurred?
2. When did the failures begin and end?
3. Which account was targeted?
4. What was the source of the attempts?
5. Did a successful login occur afterward?
6. Was the source expected?
7. Are there other suspicious events around the same timeframe?

## 📊 Evidence to Collect

| Evidence       | Purpose                            |
| -------------- | ---------------------------------- |
| Timestamp      | Build an event timeline            |
| Username       | Identify affected account          |
| Source         | Identify origin where available    |
| Result         | Confirm failed/successful attempts |
| Attempt Count  | Determine frequency                |
| Related Events | Establish context                  |

## 🧠 L1 Analysis

Repeated authentication failures can have multiple explanations:

* User error
* Incorrect stored credentials
* Misconfigured service
* Automated authentication attempts
* Potential credential attack activity

The analyst should therefore **avoid immediately classifying the activity as malicious**.

## 🔗 Correlation Strategy

```text
Failed Login Alert
       ↓
Identify Account
       ↓
Establish Timeline
       ↓
Identify Source
       ↓
Check Successful Login
       ↓
Review Related Host Activity
       ↓
Assess Context
       ↓
Determine Severity
       ↓
Escalate if Required
```

## 🚦 Triage Assessment

**Initial Severity:** Medium

**Current Status:** Requires investigation.

**Confidence:** Low until supporting evidence is reviewed.

### Possible Escalation Factors

The alert may require increased attention if investigation identifies:

* Repeated failures from an unexpected source
* A successful authentication following numerous failures
* Multiple accounts being targeted
* Unusual activity on the affected host
* Additional correlated security alerts

## 📝 Analyst Notes

**Timeline:** Pending evidence review.

**Affected Account:** `lab-user`

**Finding:** No final determination without supporting evidence.

**Escalation:** To be determined after correlation and validation.

## 🎓 Skills Demonstrated

* Authentication alert triage
* Event timeline analysis
* SIEM investigation
* Evidence collection
* Alert severity assessment
* Event correlation
* SOC Analyst L1 escalation methodology

## ⚠️ Disclaimer

This is a simulated cybersecurity lab created for educational and portfolio purposes. It does not represent a real-world security incident.
