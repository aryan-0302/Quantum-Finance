# European Call Option Pricing: Classical vs Quantum Approaches

# Introduction:
This project explores two approaches to pricing a European Call Option:
1.Classical Monte Carlo Simulation: A statistical method using random sampling to estimate the option price.
2.Quantum Algorithm: Utilizing Quantum Amplitude Estimation (QAE) for efficient and accurate pricing.

Classical Approach: Monte Carlo Simulation
Overview
Monte Carlo simulation estimates the price of a European call option by simulating potential price paths of the underlying asset and calculating the average payoff.

Key Features
Simulates asset price paths using geometric Brownian motion.
Computes the expected payoff of the call option.
Inputs
Initial Price ((S_0)): 50
Strike Price ((K)): 55
Risk-Free Rate ((r)): 0.05
Volatility ((\sigma)): 0.4
Time to Maturity ((T)): 1 year
Number of Simulations ((M)): 1000
Results
Estimated option price: 6.50 Rs
Graphical outputs:
Simulated price paths over time.
Frequency distribution of simulated end prices and option payoffs.



Quantum Approach: Quantum Amplitude Estimation (QAE)
Overview
A quantum algorithm estimates the expected payoff of the option by encoding the probability distribution of asset prices in quantum states and using QAE to estimate the expected value.

Key Features
Encodes uncertainty using a log-normal distribution.
Models the payoff function as a linear amplitude function.
Combines the uncertainty model and payoff function into a quantum circuit.
Uses iterative amplitude estimation to compute the expected payoff.
Steps
Define Parameters:

Spot Price ((S)): 50
Volatility ((vol)): 0.4
Risk-Free Rate ((r)): 0.05
Time to Maturity ((T)): 30 days
Model Uncertainty:

Compute parameters ((\mu, \sigma)) for the log-normal distribution.
Define bounds ((low, high)) for the distribution.
Construct Uncertainty Model:

Encode the log-normal distribution using quantum amplitudes.
Define Payoff Function:

Set strike price ((K)) and construct a linear amplitude function for the payoff.
Build Quantum Circuit:

Combine the uncertainty model and payoff function into a quantum circuit.
Set Up QAE Problem:

Define the estimation problem for amplitude estimation.
Perform Amplitude Estimation:

Estimate the expected payoff with specified precision ((\epsilon)) and confidence ((\alpha)).
Interpret Results:

Calculate the expected payoff, discount factor, and final option price.
Results
Exact Expected Value: 0.7483
Estimated Value: 0.8803
Estimation Error: 0.1320
Confidence Interval: [0.8534, 0.9072]
Expected Payoff at Maturity: 9.3804
Discount Factor: 0.9959
Final Option Price (Present Value): 9.3419


Conclusion
This project demonstrates the effectiveness of both classical and quantum approaches to pricing European call options. While Monte Carlo simulation is a reliable classical method, the quantum approach offers a promising alternative with the potential for faster and more accurate calculations in finance.
