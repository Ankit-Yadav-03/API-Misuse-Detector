# API Key Misuse Detector

Evidence-based **offline audits** to detect API key abuse, leakage, and misuse
using deterministic, explainable security signals.

This tool is designed for security reviews, incident response, and compliance
contexts where **clarity, evidence, and trust** matter more than real-time blocking.


## Overview

API keys are frequently leaked, misused, or abused without immediate visibility.
When incidents occur, teams often lack a clear, explainable way to determine:

- Was the key abused?
- How severe was the misuse?
- What evidence supports this conclusion?

This tool analyzes API usage logs and produces a **structured audit report**
highlighting misuse patterns with supporting evidence, enabling informed
human decision-making.


## What This Tool Does

It analyzes API usage events and detects the following misuse signals:

- **Rate Anomaly**  
  Sudden request volume spikes that may indicate leaked or abused keys.

- **Authentication Burst**  
  Bursts of 401 / 403 responses suggesting probing, brute-force attempts,
  or invalid key usage.

- **Endpoint Anomaly**  
  Unusually broad endpoint usage within a short time window, indicating
  exploratory or unintended access.

- **IP Evidence**  
  Contextual information such as distinct source IPs to support investigation,
  without making automated judgments.


## What This Tool Does NOT Do

This tool does NOT:
- Automatically block traffic
- Claim to detect all possible misuse
- Use machine learning or black-box scoring
- Make final security decisions without human review

It provides **signals and evidence** — humans make the judgment.


## Detection Signals

| Signal            | What it Indicates                            |
|-------------------|----------------------------------------------|
| Rate Anomaly      | Possible leaked key or abuse                 |
| Auth Burst        | Brute-force or invalid key usage             |
| Endpoint Anomaly  | Exploratory or unintended API usage          |
| IP Evidence       | Context to support security investigation    |


