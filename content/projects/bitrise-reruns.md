---
title: "Killing a 27% CI re-run rate"
date: 2025-03-01
description: "Local CI/CD tooling so mobile builds fail on laptops, not on Bitrise."
tags: ["ci-cd", "bitrise", "devex", "mobile"]
---

**Problem:** 27% of Bitrise mobile builds were being re-run — wasted minutes and blocked developers.

**Built:** local CI/CD tooling that reproduces the pipeline on a developer's machine, plus a fix for a CI package dependency deadlock that had blocked builds for 28 days.

**Result:** the re-run rate eliminated.
