# econ5200-lab14-ols-diagnostics
# OLS Diagnostics: Robust and Clustered Standard Errors

## Objective

I investigated how heteroskedasticity, correlated errors, and influential observations affect OLS regression results and statistical inference.

## Methodology

- I simulated data with heteroskedastic errors and compared the coverage rates of classical and HC3 confidence intervals.
- I simulated correlated errors within 40 firms and compared HC3 and clustered standard errors.
- I used leverage, studentised residuals, and Cook's distance to identify influential observations.
- I wrote a prompt asking AI to create a function that calculates different types of standard errors and checked its results against statsmodels.

## Key Findings

- Under heteroskedasticity, classical coverage was 92.4%, while HC3 coverage was 94.4%. HC3 was closer to the target of 95%.
- With correlated errors within firms, HC3 coverage was only 50.3%, while clustered coverage improved to 93.7%.
- I examined three planted observations and found that one influential observation was mainly responsible for changing the slope from 1.4927 to 1.4468.
- The AI-generated function passed all 18 checks against statsmodels in the first round.

I learned that choosing the correct standard errors is important for reliable statistical inference. I also learned that influential observations should be investigated rather than automatically removed, and AI-generated code should be checked before use.
