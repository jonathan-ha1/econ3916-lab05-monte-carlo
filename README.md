# Monte Carlo Engine -- Probability & Simulation

## Objective
Use random simulation to estimate probabilities and financial risk, and check how the accuracy of those estimates improves as the number of trials grows.

## Methodology
- Simulated 10,000 coin flips and plotted the running share of heads to show how it settles toward 0.5 as more flips are added.
- Simulated 10,000 games of the Monty Hall problem and compared how often switching doors won against how often staying won.
- Simulated a disease screening test on 100,000 people, with a prevalence of 1%, a sensitivity of 95%, and a specificity of 90%, then counted what share of positive tests came from people who were actually sick.
- Ran a Monte Carlo simulation of returns on a $1M portfolio and used the simulated losses to compute the 95% Value at Risk (VaR) and the 95% Expected Shortfall (ES).
- Estimated pi with Monte Carlo sampling at different sample sizes and checked that the error shrinks at a rate of about 1/sqrt(n).

## Key Findings
- Switching doors in Monty Hall won 6,694 of the 10,000 games.
- Only 9.2% of positive screening tests were from people who were sick. Even with a fairly accurate test, a low prevalence means most positive results are false positives.
- For the $1M portfolio, the 95% VaR was $19,494 and the 95% ES was $24,230. ES is larger because it averages the losses beyond the VaR cutoff, not just the cutoff itself.
- The error in the pi estimates fell at roughly 1/sqrt(n), so getting 10 times more accurate takes about 100 times more samples.
