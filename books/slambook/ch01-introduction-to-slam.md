# Introduction to SLAM

Chapter 1

## Summary
Role of this chapter is to gain an intuitive understanding of the modules in a SLAM system and each module's main functionality

## Robot behaviour
Describe the motion of a robot, how **x** (position) changes from time step k-1 to k, what does the sensor observe?
The instructions given to a robot are affected by noise

## The two basic SLAM equations 

- Motion: $x_k = f(x_{k-1}, u_k, w_k)$
- Observation: $z_{k,j} = h(y_j, x_k, v_{k,j}), \; (k,j) \in \mathcal{O}$

These two equations together describe the basic problem of SLAM, how to estimate **x** (localization) and **y** (mapping)
problem with the noisy input **u** 

## The solution to the state estimation problem

It is related to the specific forms of the two equations from above(motion and observation), whethere they are linear or non-linear and the distribution of the noise, whether it is Gaussian or non-Gaussian

The Linear Gaussian system is the simplest. and its unbiased optimal estimation can be  given by the Kalman Filter(KF). The more complex system is the nonlinear non-Gaussian system, which relies on two methods:
-Extended Kalman FIlter (EKF)
-nonlinear optimization 

We linearize the system then we solve it in 2 steps: predict-update