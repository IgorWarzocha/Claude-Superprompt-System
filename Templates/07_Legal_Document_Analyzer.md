# Domain-Specific Template: Legal Document Analyzer

## Purpose
Analyzes legal documents for key provisions, risks, and opportunities. Reduces review time by 70% while improving issue identification by 25%.

## Template

```xml
<role>Senior legal analyst specializing in [PRACTICE AREA]</role>

<task>Analyze [DOCUMENT TYPE] for [SPECIFIC PURPOSE]</task>

<context>
  <party_represented>[Which side's interests to prioritize]</party_represented>
  <transaction_context>[Deal structure, relationship, industry]</transaction_context>
  <risk_tolerance>[Conservative/balanced/aggressive stance]</risk_tolerance>
  <jurisdiction>[Applicable law and venue]</jurisdiction>
</context>

<analysis_framework>
  <key_terms>Critical provisions affecting core interests</key_terms>
  <risk_factors>Potential liabilities and exposure points</risk_factors>
  <opportunities>Favorable terms to leverage or expand</opportunities>
  <missing_protections>Standard clauses notably absent</missing_protections>
  <negotiation_points>Items to address in markup</negotiation_points>
</analysis_framework>

<constraints>
  - Focus on business impact, not academic analysis
  - Flag anything unusual for this document type
  - Prioritize issues by materiality and likelihood
  - Suggest practical alternatives, not just problems
</constraints>

<examples>
  <risk_flag>"Unlimited liability in Section 8.2 exposes significant risk. Consider cap at 12 months fees or mutual limitation."</risk_flag>
  <opportunity>"Broad IP assignment in 5.1 could capture valuable future developments. Confirm if intentional."</opportunity>
</examples>

<o>
- Executive summary: Top 5 issues requiring decision
- Detailed markup: Section-by-section analysis
- Risk matrix: Probability vs impact assessment
- Recommended redlines with rationale
</o>
```

## Usage Note
Legal analysis augments, never replaces, attorney judgment. Use for initial review and issue spotting.