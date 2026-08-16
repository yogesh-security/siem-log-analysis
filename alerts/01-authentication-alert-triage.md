# 🚨 Lab 01 — Authentication Alert Triage

## 🎯 Objective

Practice the initial triage of an authentication-related security alert from a SOC Analyst L1 perspective.

> This is a simulated educational scenario and does not represent a real security incident.

## 📌 Alert Scenario

A SIEM generates an alert after detecting multiple failed authentication attempts against a user account within a short period.

### Alert Details

| Field       | Value                                   |
| ----------- | --------------------------------------- |
| Alert Type  | Multiple Failed Authentication Attempts |
| Severity    | Medium                                  |
| Status      | Open                                    |
| User        | `lab-user`                              |
| Host        | `LAB-WORKSTATION`                       |
| Source      | Simulated                               |
| Environment | Authorized Lab                          |

## 🔎 Initial Triage

The L1 analyst should first validate:

* Is the alert based on genuine authentication events?
* Which account is affected?
* Which host generated the events?
* When did the activity occur?
* How many failed attempts were recorded?
* Is there a successful login associated with the activity?
* Is the source expected?

## 📊 Evidence to Review

Relevant authentication logs should be examined for:

* Timestamp
* Username
* Source address, where available
* Authentication result
* Number of attempts
* Related successful authentication
* Other events occurring around the same timeframe

## 🧠 Analyst Reasoning

Multiple failed authentication events can have several explanations, including:

* User entering an incorrect password
* Misconfigured application or service
* Automated authentication attempts
* Potential credential-related attack activity

Therefore, the alert should **not automatically be classified as malicious** without additional context.

## 🚦 Triage Decision

**Initial Severity:** Medium

**Current Assessment:** Requires investigation.

### Recommended Next Steps

1. Review the authentication events.
2. Establish the event timeline.
3. Identify the source of the attempts.
4. Check whether a successful authentication followed the failures.
5. Review related activity on the affected host.
6. Determine whether the activity is expected.
7. Escalate according to the organization's incident-response process if suspicious activity is confirmed.

## 📝 Analyst Notes

**Finding:** Pending evidence review.

**Confidence:** Low until supporting log evidence is available.

**Escalation:** Not determined at initial triage.

## 🎓 Skills Demonstrated

* SIEM alert triage
* Authentication event analysis
* Severity assessment
* Evidence collection
* Timeline analysis
* SOC L1 investigation methodology

## ⚠️ Disclaimer

This is a simulated lab scenario created for cybersecurity education and portfolio development. It does not represent a real-world security incident.
