# ISTA-Algorithm-in-Python

ISTA (Iterative Soft-Thresholding Algorithm) is a simple and easy-to-implement method for solving the BPDN (Basis Pursuit Denoising) problem. Although it may not be the best solution, it serves as a good starting point for understanding optimization in this field.

The ISTA algorithm is commonly represented as follows:

**Input:**
- `A` ∈ ℝᵐˣⁿ
- `y` ∈ ℝᵐ
- Initialize: `x₀` ∈ ℝⁿ

**While not converged, repeat:**
1. `xₖ₊₁` := S(λ/L) (xₖ - L₁ₐₜ(Aᵀ(Axₖ - y)))
2. Update `xₖ := xₖ₊₁`

**Return:**
- `xₖ₊₁`

Here, `Sₐ` represents the soft-thresholding operator with the cutoff parameter `α`. We will now derive the ISTA algorithm by initially deriving the Proximal Gradient Method, which is a fixed-point iteration, and then demonstrate how ISTA is a specific case of it.

**ISTA_FISTA**
Here I have attempted to solve basic linear regression problem through ISTA and FISTA and also attempted to solve an ODE

**ISTA_Algorithm**
Here I have discussed optimization procedure through ISTA 
