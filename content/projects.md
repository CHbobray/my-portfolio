---
title: "Projects"
hidemeta: true
disableShare: true
ShowToc: true
---

Data science and data engineering projects from my work and my M.S. in Data Science at Northwestern University. Each project links to its code, report, or presentation.

## Personal Portfolio Website

**Tools:** Hugo, Go templates, Markdown, Git, GitHub  
This site, built with the Hugo static site generator and deployed automatically from GitHub.  
{{< doc file="https://github.com/CHbobray/my-portfolio" label="View the code on GitHub" >}}

## The Battle for Warner Bros. Discovery: A Valuation Analysis

**Type:** Team project (Group 3), February 2026  
**Methods:** Discounted cash flow (DCF), comparable company analysis, precedent transactions, sensitivity analysis

Evaluated whether Netflix's $82.7B bid ($27.75/share) or Paramount Skydance's $108B all-cash bid ($31.00/share) for Warner Bros. Discovery could be justified.

- Built a 5-year free cash flow forecast for WBD's HBO and studio assets using an 8.9% WACC, with a WACC x terminal-growth sensitivity table spanning $52B to $93B in enterprise value.
- Applied peer trading multiples (Disney, Comcast, Paramount, Lionsgate, AMC Networks) to set an implied value of $76B to $95B at 8x to 10x EV/EBITDA.
- Benchmarked five media M&A precedents, including Disney/21st Century Fox and AT&T/Time Warner, adjusting historical multiples for cord-cutting and higher interest rates.
- Assessed each bidder's financing capacity, debt headroom, and credit risk.

**Conclusion:** Netflix's bid falls within the valuation range and is financeable. Paramount's bid exceeds intrinsic value under every method and would push combined leverage above 10x EBITDA.

{{< doc file="/projects/WBD-Valuation-Analysis.pdf" label="View the presentation (PDF)" >}}

## Moz at a Crossroads: Diagnosing Unsustainable Growth

**Type:** Team case analysis (Group 3), based on the Harvard Business School case "Rand Fishkin at Moz"  
**Methods:** Financial trend analysis, sustainable growth rate (SGR) framework, root cause diagnosis, strategic recommendations

Analyzed why Moz, an SEO software company, nearly doubled revenue from $21.9M to $42M between 2012 and 2016 while burning $31.2M in cash, leading to layoffs of 59 of 210 employees.

- Charted ten years of revenue against annual cash generation to expose the gap between headline growth and cash burn, including a $12M loss in the first full year of expansion.
- Diagnosed four compounding root causes: acquisition spending over retention (average subscriber tenure of 11 months), premature product expansion, rising organizational complexity as headcount grew to 210, and lost competitive position in core SEO.
- Applied the sustainable growth rate framework (profit margin, earnings retention, asset turnover, financial leverage) to show why Moz's growth outpaced what its financial structure could fund.
- Recommended a sequenced turnaround: refocus on the core Moz Pro product, fix retention before scaling acquisition, and anchor growth targets to internally generated cash.

{{< doc file="/projects/Moz-Growth-Analysis.pdf" label="View the presentation (PDF)" >}}

## College Scorecard EDA: Do College Costs Pay Off?

**Tools:** Python, pandas, NumPy, Matplotlib, seaborn, Jupyter  
**Data:** U.S. Department of Education College Scorecard (6,429 institutions, 3,306 fields)

Explored how completion rate, tuition, student debt, institution type, and enrollment size relate to graduates' median earnings 10 years after entry.

- Profiled missing values and privacy-suppressed codes, used boxplots and the IQR method to separate legitimate outliers from invalid data, and engineered new fields (tuition gap, enrollment size bins, earnings-to-debt ratio).
- Cleaned the data down to 1,938 institutions with complete key fields.
- Tested three hypotheses with correlation and regression plots: completion rate (r = 0.51) was the strongest predictor of earnings, ahead of tuition and debt (both r = 0.47).
- Compared institution types: public schools delivered median earnings of about $49,300 at about $8,500 tuition, while for-profit schools had the lowest earnings (about $40,100) at twice the public tuition.

{{< doc file="https://github.com/CHbobray/college-scorecard-eda" label="View the notebook and code on GitHub" >}}

## Production Planning Optimization (MSDS 460: Decision Analytics)

**Tools:** Python, PuLP, GLPK solver, pandas  
**Type:** Team project, Northwestern University, August 2026

Built a multi-period linear programming model for a manufacturer producing three products at two plants over five periods, choosing production, inventory, labor, overtime, advertising, and shipping to maximize profit while meeting contract demand.

- Formulated the objective, decision variables, and constraints (inventory balance, demand, labor, raw materials, storage, and advertising budget), then verified the solution with automated constraint checks.
- The baseline model produced an optimal profit of $7.07M on $8.48M in revenue.
- Scenario analysis showed Raw Material 1 was the critical bottleneck: a 25% increase added $63,295 in profit, versus $20,559 for more Plant B labor and $0 for a larger advertising budget.
- Sensitivity analysis found that a small increase in Raw Material 1 captured nearly all of the available gain before other constraints took over.
- An integer programming version requiring whole-unit production reduced profit by only $254 (0.004%), confirming the continuous model's plan was practical.

{{< doc file="/projects/NU-Production-Optimization.pdf" label="Read the full report (PDF)" >}}
{{< doc file="https://github.com/CHbobray/nu-production-optimization" label="View the code on GitHub" >}}




