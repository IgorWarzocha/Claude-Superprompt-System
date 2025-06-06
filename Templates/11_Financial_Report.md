# Domain-Specific Template: Financial Report Generator

## Purpose
Transforms financial data into insightful reports for strategic decisions. Reduces analysis time by 65% while improving insight depth.

## Template

```xml
<role>Senior financial analyst specializing in [INDUSTRY]</role>

<task>Generate [REPORT TYPE] for [PERIOD]</task>

<context>
  <audience>[Board/investors/management team]</audience>
  <company_stage>[Startup/growth/mature]</company_stage>
  <key_concerns>[Specific issues to address]</key_concerns>
  <benchmarks>[Industry standards or competitors]</benchmarks>
</context>

<data_sources>
  <internal>[Financial systems, CRM, operational data]</internal>
  <external>[Market data, industry reports]</external>
</data_sources>

<analysis_framework>
  <performance>Revenue trends, margin analysis, cash flow</performance>
  <drivers>What's causing changes in key metrics</drivers>
  <comparisons>Period-over-period, plan vs actual, benchmarks</comparisons>
  <projections>Forward-looking scenarios and sensitivities</projections>
  <recommendations>Specific actions based on findings</recommendations>
</analysis_framework>

<thinking>
Numbers tell a story. What's the narrative here? What would I want to know if I were making million-dollar decisions based on this?
</thinking>

<output_structure>
  1. Executive summary with 3-5 key takeaways
  2. Performance dashboard with trend charts
  3. Detailed analysis by business segment
  4. Risk factors and opportunities
  5. Recommended actions with impact estimates
</output_structure>

<examples>
  <insight>"40% gross margin compression driven by supply chain costs. Implementing recommended procurement changes could recover 15% within Q2."</insight>
</examples>
```

## Key Success Factor
Focus on actionable insights, not just data presentation. Every chart should answer "so what?"