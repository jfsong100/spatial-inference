# Spatial Linear Mixed Effects Models

This website demonstrates methods for inference in:

\[
y = X\beta + w + \epsilon, \quad w \sim \mathcal{GP}(0, C), \quad \epsilon \sim \mathcal{N}(0, \tau^2)
\]

with \( C_{ij} = \exp(-\phi \| s_i - s_j \|) \).

## 🔧 Simulation Code

We use BRISC to simulate spatial processes efficiently. See `scripts/simulate_data.R`.

```r
# Preview:
set.seed(1010)
n <- 1000
s <- cbind(runif(n, 1, 5), runif(n, 1, 5))
# ... (see full script in repository)
