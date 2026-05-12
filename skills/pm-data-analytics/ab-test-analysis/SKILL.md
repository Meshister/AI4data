---
name: ab-test-analysis
description: Analyze A/B test results with statistical significance, sample size validation, confidence intervals, and ship/extend/stop recommendations. Use when evaluating experiment results, checking if a test reached significance, interpreting split test data, or deciding whether to ship a variant.
---

# A/B Test Analysis

Evaluate A/B test results with statistical rigor and translate findings into clear product decisions.

## Context

You are analyzing A/B test results for **$ARGUMENTS**.

If the user provides data files (CSV, Excel, or analytics exports), read and analyze them directly. Generate Python scripts for statistical calculations when needed.

## Instructions

1. **Understand the experiment**: Document hypothesis, variant changes, primary and guardrail metrics, test duration, and traffic split.

2. **Validate the test setup**: Check sample size using n = (Z²α/2 × 2 × p × (1-p)) / MDE², verify duration covers 1-2 business cycles, assess randomization quality, and evaluate novelty effects.

3. **Calculate statistical significance**: Determine conversion rates, relative lift, p-value (two-tailed z-test or chi-squared), 95% confidence intervals, and assess both statistical and practical significance.

4. **Check guardrail metrics**: Verify no degradation in revenue, engagement, or performance indicators.

5. **Interpret results**: Apply decision framework mapping outcomes (significant positive, positive trend, flat, negative) to recommendations (Ship/Extend/Stop/Investigate).

6. **Provide analysis summary** in markdown table format with metrics, control/variant values, lift, p-values, and clear recommendations with reasoning.

## Further Reading

- A/B Testing 101 + Examples
- Testing Product Ideas: The Ultimate Validation Experiments Library
- Are You Tracking the Right Metrics?
