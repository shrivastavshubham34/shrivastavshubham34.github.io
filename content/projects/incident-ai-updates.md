---
title: "AI-written incident updates (Lambda + Gemini)"
date: 2025-09-01
description: "Zenduty incident telemetry → AWS Lambda → Google Gemini → plain-language stakeholder updates."
tags: ["sre", "incident-response", "aws-lambda", "ai"]
---

**Problem:** during incidents, engineers were translating alerts into updates for non-technical stakeholders by hand — while also fixing the incident.

**Built:**
- Led the company-wide move from PagerDuty to Zenduty.
- An AWS Lambda that takes incident telemetry and uses Google Gemini to draft stakeholder-friendly status updates.

**Result:** engineers fix, the bot explains.
