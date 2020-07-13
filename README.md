# limit-cycle

The main functions implemented in "Limit_Cycle_Maple_Code" are

# NormalForm(P, Q, p, q, k)

-Computes the normal form of averaging up to k-th order in epsilon

--P and Q are polynomials in a considered planar differential system which has a center at the origin (from equation (2.1))

--p and q are polynomials in the perturbations of a differential system (from equation (2.2))

--k is the order in epsilon from the normal form of averaging (2.3) (usually called the averaging order)


# DSolutions(F_0)

-Computes the 2\pi-periodic solution r(theta,z) of the unperturbed system dr/d theta=F_0(theta,z) with initial condition r(0,z)=z, a set of inequalities (SIs) with respect to z, and the fundamental solution Y(theta,z) of the variational equation Y'=\partial F_0(\theta,r(\theta,z))Y with initial condition Y(0,z)=1

--F_0 is the unperturbed term obtained from the function NormalForm(P,Q,p,q,k)

Note: the open and bounded interval D can be determined by using the output set SIs

# AveragingFormula(k)

-Computes the exact formula of the k-th order intergal function y_k(theta,z)

--k is the averaging order

# AveragedFunction(dr/d theta, r(theta,z), Y(theta,z), k)

-Computes a list of expressions of the averaged functions

--dr/d theta is the normal form of averaging obtained from the function NormalForm(P,Q,p,q,k)

--r(theta,z) and Y(theta,z) are the fundamental solutions obtained from the function DSolutions(F_0)

--k is the averaging order

# Support

The codes are supported by China Scholarship Council (#201806020128).
