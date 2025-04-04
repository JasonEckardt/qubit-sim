---
tags:
  - quantum-mechanics
---

# 1.1 The Original Stern-Gerlach Experiment

## Magnetic Moment and Angular Momentum of a Particle

Classically, $L=r\times p$ is the angular momentum of a particle. For the Earth, $L=I\omega$ due to the orbit the Earth takes. However, these are just different forms of $L$.

To express the relationship between angular moment of a charged particle and its magnetic moment, consider a point particle with charge $q$ and mass $m$ moving in a circular orbit $r$ with speed $v$.

![[PHYS375-Orbiting-Charged-Particle-Visual.excalidraw]]

The magnetic moment of $\mu$ is given by
$$
\mu=\frac{IA}{c}
$$
where $A$ is the area of the circle formed by the orbit and the current $I$ is the charge $q$ divided by the period $T=2\pi r/v$.

> Note that $c$ is a constant to convert SI units to Gaussian units.

You can rewrite $\mu$ as
$$
\mu=\frac{q}{T}\frac{\pi r^2}{c}=\frac{qv}{2\pi r}\frac{\pi r^2}{c}=\frac{qvr}{2c}
$$

Introducing the orbital angular momentum $L=mvr$ yields
$$
\mu=\frac{qvr}{2mvrc}L=\frac{q}{2mc}L\tag{1.1}
$$
Thus we can express the relationship between $\mu$ and $L$ as
$$
\mu=\frac{q}{2mc}L\tag{1.2}
$$

**Example**: Consider a solid sphere with a magnetic charge $q$ distributed uniformly on its surface. The sphere has a constant of proportionality of $5q/6mc$.

## Intrinsic Spin Angular Momentum of a Particle

To express the intrinsic spin angular momentum of a particle, we write
$$
\mu=\frac{gq}{2mc}S\tag{1.3}
$$

where $g$ is experimentally determined to be
$g=2.00$ for an electron,
$g=5.58$ for a proton,
and $g=-3.82$ for a neutron.

> You can think of $g$ as a dimensionless factor that outputs the correct magnitudes and units. 

## The Stern-Gerlach Experiment

The experiment uses an oven to evaporate silver atoms and produce a collimated beam of silver atoms.

A series of slits are placed in front of the oven to only select the silver atoms. The beam is then directed between two magnets. 

One of the magnets is flat while the other has a sharp tip. 
This creates an inhomogeneous magnetic field.

![[PHYS375-Figure-1.1.png]]

When a *neutral* atom with magnetic moment $\mu$ enters the magnetic field $B$, it experiences a force $F=\triangledown(\mu\cdot B)$.

Calling the direction in which the inhomogeneous magnetic field is largest, in this case, the $z$ axis, we can see that
$$
F=\mu\cdot\frac{\partial B}{\partial z}\cong\frac{\partial B_z}{\partial z}\tag{1.4}
$$

In the figure, the magnetic field gradient $-\partial B/\partial z$, so that if $-\mu_z$, $F_z$ is positive.
As a result, the atoms are deflected upwards, or in the positive $z$ direction.

The result of this experiment is unlike the natural expectation that $\mu$ takes on values between $\pm\mu$, it only takes on two values!

Namely, $\mu=\pm h/2$. These two discrete values are called *spin-up* and *spin-down*.
Numerically, $h=h/2\pi=1.055\times10^{-27}erg\cdot s=6.582\times10^{-16}eV\cdot s$, where $h$ is [[Planck's Constant]].

# 1.2 Four Experiments

![[PHYS375-Figure-1.3.png]]

## Experiment 1

### The Ket Vector

The symbol $\ket{+z}$ is known as a **ket vector**.

Consider a particle that exits an SG$z$ device, with its inhomogeneous magnetic field parallel to the $z$ axis with $S_z=h/2$. Then $S_z$ is in the state $\ket{+z}$.

### Result of Experiment 1

Suppose a beam of particles, *each* is in the state of $\ket{+z}$ enters an SG$z$ device. We find that *all* of the particles exit in the same state of $\ket{+z}$ which means $S_z=h/2$ for each of the particles.

## Experiment 2

Consider the same beam of particles that exit the SG$z$ device. 

Suppose they enter another SG$x$ device, that is, a device such that the inhomogeneous magnetic field is parallel to the $x$ axis.

We find that 50% exit the SG$x$ device with $S_x=h/2$ and in the state of $\ket{+x}$, while the other 50% exit with $S_x=-h/2$ and in the state of $\ket{-x}$. 

## Experiment 3

Adding a third SG$z$ device, a device where the inhomogeneous magnetic field is parallel to the $z$ axis.

If we send the beam of particles exiting the SG$x$ device into the SG$z$ device, we find that 50% exit in the state of $\ket{+z}$ and 50% exit in the state of $\ket{-z}$, although none of the particles initially entered in the state of $\ket{-z}$!

$S_z$ and $S_x$ are incompatible observables. We cannot know both of them simultaneously.

## Experiment 4

![[PHYS375-Figure-1.4.png]]

The second modified magnet pushes a particle with a magnetic moment in the opposite direction of the first magnet.

As a result, the particle is decelerated and brought in the transverse direction in the first half of the second magnet. At the second half of the magnet, the particle is accelerated back toward its original axis.

The net effect of the three magnets is to recombine the beams so that their condition on exiting the devices is the same as they initially entered in.

### A Modified SG Device

![[PHYS375-Figure-1.5.png]]

With the modified SG device, we can select a particular particle.

Consider the modified SG device oriented along the $x$ axis, we can select a particle in the $\ket{+x}$ spin state by blocking the path for the $\ket{-x}$. 

As a result, all of the particles exiting the SG$x$ device would be in the state $\ket{+x}$.

If the $\ket{-x}$ is filtered out in Experiment 3, we find the same result for the SG$z$ device!
That is, 50% exit the SG$z$ device in the state $\ket{+z}$ and the other 50% exit in the state $\ket{-z}$.
Similarly, if we block the $\ket{+x}$, we will reach the same result.

### Result of Experiment 4

A beam of particles in the state $\ket{+z}$ enters an SG$x$ device but neither of the paths are being blocked, and therefore does not take a measurement of $S_x$.

The beam is then sent into another SG$z$ device and find that 100% of the particles exit the SG$z$ device in the state $\ket{+z}$.

![[PHYS375-Figure-1.6.png]]

A **probability amplitude** is "squared" to get the probability of a particle entering in a specific state.

> When we *don't* make a measurement in the modified SG device, we must add the amplitudes, *not* the probabilities.


# 1.3 The Quantum State Vector

In Experiment 1, when we initially send a particle in the initial state of $\ket{+z}$, there is a zero amplitude for the particle to be found in the $\ket{-z}$ state, which we denote
$$
\braket{-z|+z}=0=\braket{+z|-z}
$$

We can think of these two vectors of being orthogonal which is analogous to $i\cdot j=0$ in an electric field.

If we send a particle in the state of $\ket{+z}$ into an SG$z$ device, we will find the particle in the state $\ket{+z}$. In quantum amplitudes, this says that $\braket{+z|+z}$ is nonzero.

It is convenient for these vectors to be unit vectors and satisfy
$$
\braket{+z|+z}=1
$$
and similarly,
$$
\braket{-z|-z}=1
$$

just as $i\cdot i=1$ and $j\cdot j=1$ in an electric field.

![[PHYS375-Figure-1.7.png]]

Suppose a particle in the state $\ket{+x}$, then the particle has nonzero amplitudes in the states of $\ket{+z}$ and $\ket{-z}$, which we can call $c_+$ and $c_-$ respectively.

We can express this state as
$$
\ket{+x}=c_+\ket{+z}+c_-\ket{-z}
$$
a linear combination of the states $\ket{+z}$ and $\ket{-z}$.

An arbitrary spin state $\ket{\psi}$, which is created by sending a particle into an SG device where the inhomogeneous magnetic field oriented in an arbitrary direction.

In general, this state $\ket{\psi}$ will have nonzero amplitudes to yield both $h/2$ and $-h/2$ if $S_z$ is measured. Thus we can express $\ket{\psi}$ as
$$
\ket{\psi}=c_+\ket{+z}+c_-\ket{-z}\tag{1.5}
$$
^15

where $c_+$ and $c_-$ depend on the orientation of the SG device.

An arbitrary state $\ket{\psi}$ can be expressed as a superposition of the states $\ket{+z}$ and $\ket{-z}$ and therefore form a **complete set**, similar to $i,j,k$ forming a complete set in an electric field $E$.

## The Bra Vector

For every ket vector for an arbitrary state $\ket{\psi}$, there exists a corresponding **bra vector** $\bra{\psi}$.

Thus there are two ways to represent $S_z=h/2$, denoted either in the state $\ket{+z}$ or $\bra{+z}$.

Bras and kets form an *amplitude* or *inner product* $\braket{\varphi|\psi}$ to form a bracket.

The amplitude $\braket{\varphi|\psi}$ is the probability for a particle in the state $\ket{\psi}$ to be found in $\ket{\varphi}$.

From earlier experiments, we know that
$$
\braket{-z|+z}=0=\braket{+z|=z}=0
$$
since a particle in the state $\ket{=z}$, with $S_z=-h/2$, has zero amplitude to be found in the state $\ket{+z}$, with $S_z=h/2$.

From [[#^15]] we can deduce that
$$
\begin{align*}
\braket{+z|\psi}=c_+\braket{+z|+z}+c_-\braket{+z|-z}=c_+\\
\braket{-z|\psi}=c_+\braket{-z|+z}+c_-\braket{-z|-z}=c_-
\end{align*}
\tag{1.6ab}
$$
^16ab

or $c_\pm=\braket{\pm z|\psi}$.

We can express $\ket{\psi}$ as
$$
\begin{align*}
\ket{\psi}=\braket{+z|\psi}\;\ket{+z}+\braket{-z|\psi}\;\ket{-z}\\
=\ket{+z}\braket{+z|\psi}+\ket{-z}\braket{-z|\psi}
\end{align*}
\tag{1.7}
$$
^17

> Note: The amplitudes are $\braket{+z|\psi}$ and $\braket{-z|\psi}$ are complex numbers, and thus the product of an amplitude times a ket vector is just a ket vector.

Since for every ket, there corresponds a bra vector, we must be able to express $\bra{\psi}$ in terms of $\bra{+z}$ and $\bra{-z}$ as
$$
\bra{\psi}=c'_+\bra{+z}+c'_-\bra{-z}\tag{1.8}
$$

From $\bra{\psi}$ we can deduce that
$$
\begin{align*}
\braket{\psi|+z}=c'_+\\
\braket{\psi|-z}=c'_-
\end{align*}
\tag{1.9ab}
$$
^19ab

Thus we can define $\bra{\psi}$ as
$$
\bra{\psi}=\braket{\psi|+z}\;\bra{+z}+\braket{\psi|-z}\;\bra{-z}\tag{1.10} 
$$

^110

## Complex Conjugates

The amplitudes $\braket{+z|\psi}$ and $\braket{\psi|+z}$ are related.

To show this, we will need $\braket{+z|+z}=1$ and $\braket{\psi|\psi}=1$.
We can evaluate $\braket{\psi|\psi}$ using [[#^17]] and [[#^110]] to find
$$\begin{align*}
\braket{\psi|\psi}=\braket{\psi|+z}\braket{+z|\psi}\braket{+z|+z}+\braket{\psi|-z}\braket{-z|\psi}\braket{-z|-z}\\
=\braket{\psi|+z}\braket{+z|\psi}+\braket{\psi|-z}\braket{-z|\psi}\\
=1
\end{align*}
\tag{1.11}
$$
^111

The amplitudes $\braket{+z|\psi}$ and $\braket{-z|\psi}$ are in general complex numbers. The way to guarantee [[#^111]] for any arbitrary $\ket{\psi}$ is to have
$$
\braket{\psi|+z}=\braket{+z|\psi}^*\;\;\;\mathsf{and}\;\;\;\braket{\psi|-z}=\braket{-z|\psi}^*
\tag{1.12}
$$

so that each of the terms in [[#^111]] is real.

This is to say that the amplitude for a particle in the state $\ket{\psi}$ to be found in the states $\ket{\pm z}$ is the *complex conjugate* of the amplitude for a particle in the states $\ket{\pm z}$ to be found in the state $\ket{\psi}$.  

From [[#^16ab]] and [[#^19ab]], we can see that $c'_+=c^*_+$ and $c'_-=c^*_-$. Therefore, the bra corresponding to the ket [[#^15]] is
$$
\bra{\psi}=c^*_+\bra{+z}+c^*_-\bra{-z}
\tag{1.13}
$$
^113

The bra is generated by the ket vector by changing all the basis kets to their corresponding bra vectors and by changing all of the amplitudes (complex numbers) to their complex conjugates.

We can express [[#^111]] as

$$
\begin{align*}
\braket{\psi|\psi}=\braket{+z|\psi}^*\braket{+z|\psi}+\braket{-z|\psi}^*\braket{-z|\psi}\\
=c^*_+c_++c^*_-c_-=1
\end{align*}
\tag{1.14}
$$
^114

or as
$$
\braket{\psi|\psi}=\left|\braket{+z|\psi}\right|^2+\left|\braket{-z|\psi}\right|^2=1
\tag{1.15}
$$
^115

where
$$
\begin{align*}
\braket{+z|\psi}^*\braket{+z|\psi}\equiv\left|\braket{+z|\psi}\right|^2\\
\braket{-z|\psi}^*\braket{-z|\psi}\equiv\left|\braket{-z|\psi}\right|^2
\end{align*}
$$

We interpret $\left|\braket{\pm z|\psi}\right|$ as the probability of a particle in the state $\ket{\psi}$ to be found in the state $\ket{\pm z}$ if a measurement of $S_z$ is made with an SG$z$ device.

As [[#^115]] shows, the requirement that $\braket{\psi|\psi}=1$ guarantees that the probability of finding the particle in one state or the other sums to $1$ since there are only two results possible for the measurement of $S_z$ in a spin-$\frac{1}{2}$ particle.

When both of the probability amplitudes $\braket{+z|\psi}$ and $\braket{-z|\psi}$ of [[#^17]] is nonzero, then a particle in the state $\ket{\psi}$ is in a **superposition** of the states $\ket{+z}$ and $\ket{-z}$.

There are probabilities of obtaining both $S_z=h/2$ and $S_z=-h/2$ if a measurement is taken.

On the contrary to classical mechanics, where a particle is in a definite state, we do not expect two measurements of the orbital angular momentum of the particle in a particular time to yield two different values such as $r_1\times p_1$ and $r_2\times p_2$.

## Example 1.1

A measurement of $S_z$ is carried out on a particle in the state
$$
\ket{\psi}=\frac{1}{2}\ket{+z}+\frac{i\sqrt{3}}{2}\ket{-z}
$$

What are the possible results of this measurement and with what probability do these results occur?

---

To find the probability of $\ket{+z}$, we will get the dot product $\braket{+z|\psi}$.
$$
\braket{+z|\psi}=\frac{1}{2}\braket{+z|+z}+\frac{i\sqrt{3}}{2}\braket{+z|-z}
$$

Since $\braket{+z|+z}=1$ and $\braket{+z|-z}=0$, we find that
$$
\begin{align*}
\braket{+z|\psi}=\frac{1}{2}\\
\lvert\braket{+z|\psi}\rvert^2=\frac{1}{4}
\end{align*}
$$
Therefore the probability amplitude of a particle entering in the state of $\ket{+z}$ is $1/4$ or a 25% chance of $S_z=h/2$.

Similarly,
$$
\begin{align*}
\braket{-z|\psi}=\frac{1}{2}\braket{-z|+z}+\frac{i\sqrt{3}}{2}\braket{-z|-z}
\end{align*}
$$

Since $\braket{-z|+z}=0$ and $\braket{-z|-z}=1$, we find that
$$
\begin{align*}
\braket{-z|\psi}=\frac{i\sqrt{3}}{2}\\
\lvert\braket{-z|\psi}\rvert^2=\frac{-i\sqrt{3}}{2}\cdot\frac{i\sqrt{3}}{2}=\frac{3}{4}
\end{align*}
$$

> The ket $\ket{-z}$ has a complex coefficient $i\sqrt{3}/2$, and when taking the inner product $\braket{-z|-z}$, the complex conjugate factor $c^*_-=-i\sqrt{3}/2$. 

Therefore the probability amplitude of a particle entering in the state of $\ket{-z}$ is $3/4$ or a 75% chance of $S_z=-h/2$.

Since the state $\ket{\psi}$ is "normalized", namely,
$$
\braket{\psi|\psi}=\lvert\braket{+z|\psi}\rvert^2+\lvert\braket{-z|\psi}\rvert^2=\frac{1}{4}+\frac{3}{4}=1
$$

These probabilities sum to $1$ since the only results of $S_z$ for the spin-$\frac{1}{2}$ particle are $h/2$ and $-h/2$. 

# 1.4 Analysis of Experiment 3

Experiment 3 tells us that a particle in the state $\ket{+x}$ is in a superposition of the states $\ket{+z},\ket{-z}$ such that $\ket{+x}=c_+\ket{+z}+c_-\ket{-z}$.

When we make measurements of $S_z$ with the last SG$z$ device, we have probabilities of obtaining both $h/2,-h/2$.

Because the probabilities are each 50% and from [[#^114]], we have
$$
\begin{align*}
c_+^*c_+=\braket{+z|+x}^*\braket{+z|+x}=\left|\braket{+z|+x}\right|^2=\frac{1}{2}\\
c_-^*c_-=\braket{-z|+x}^*\braket{-z|+x}=\left|\braket{-z|+z}\right|^2=\frac{1}{2}
\end{align*}
\tag{1.16ab}
$$
^116ab

We can choose $c_+$ and $c_-$ to be real, namely, $c_+=1/\sqrt{2}$ and $c_-=-1/\sqrt{2}$.
A general solution for $c_+$ and $c_-$ may be written as
$$
c_+=\frac{e^{i\delta_+}}{\sqrt{2}}\;\;\;\mathsf{and}\;\;\;c_-=\frac{e^{i\delta_-}}{\sqrt{2}}
\tag{1.17}
$$
^117

where $\delta_+,\delta_-$ are real phases that allow for the possibility for $c_+,c_-$ to be complex.
Therefore, the ket for the state with $S_x=h/2$ is given by
$$
\ket{+x}=\frac{e^{i\delta_+}}{\sqrt{2}}\ket{+z}+\frac{e^{i\delta_-}}{\sqrt{2}}\ket{-z}
\tag{1.18}
$$
^118

Note that the probabilities in [[#^116ab]] do not give any information about the values of $\delta_+,\delta_-$, since these phases cancel out when we calculate $c^*_+c_+$ and $c^*_-c_-$.
$$
\begin{align*}
c^*_+c_+=\left(\frac{e^{-i\delta_+}}{\sqrt{2}}\right)\left(\frac{e^{i\delta_+}}{\sqrt{2}}\right)=\frac{1}{2}\\
c^*_-c_-=\left(\frac{e^{i\delta_-}}{\sqrt{2}}\right)\left(\frac{e^{-i\delta_-}}{\sqrt{2}}\right)=\frac{1}{2}
\end{align*}
\tag{1.19ab}
$$
^119ab

We can use these probabilities from [[#^16ab]] to calculate the average value, or **expectation value** of $S_z$, $\braket{S_z}$.

## Expectation Value

The *expectation value* is the sum of each value obtained by a value of $S_z$ multiplied by the probability of obtaining that value.
$$
\begin{align*}
\braket{S_z}=c^*_+c_+\left(\frac{h}{2}\right)+c^*_-c_-\left(-\frac{h}{2}\right)\\
=\frac{1}{2}\left(\frac{h}{2}\right)+\frac{1}{2}\left(-\frac{h}{2}\right)\\
=\frac{h}{4}+\left(-\frac{h}{4}\right)=0
\end{align*}
\tag{1.20}
$$
^120

In this case, neither of the two values is favored. Both values have a 50% chance of being measured for $S_z$.

## Uncertainty

![[PHYS375-Figure-1.8.png]]

There is an **uncertainty** in the result of the measurements, since the measurements do not all yield the same value.

We calculate the *uncertainty* by computing the standard deviation:
1. We determine the average value of the data,
2. take each data point,
3. subtract the average value from it,
4. square and average,
5. and take the square root.

Thus the square of the uncertainty is given by
$$
\begin{align*}
(\Delta S_z)^2=\braket{(S_z-\braket{S_z})^2}\\
=\braket{S_z^2-2S_z\braket{S_z}\braket{S_z}^2}\\
=\braket{S^2_z}-2\braket{S_z}\braket{S_z}+\braket{S_z}^2\\
=\braket{S^2_z}-\braket{S_z}^2
\end{align*}
\tag{1.21}
$$
^121

The expectation value $\braket{S^2_z}$ is the sum of each value of $S^2_z$ multiplied by the probability of obtaining that value:
$$
\begin{align*}
\braket{S^2_z}=c^*_+c_+\left(\frac{h}{2}\right)^2+c^*_-c_-\left(\frac{-h}{2}\right)^2\\
=\frac{1}{2}\left(\frac{h^2}{4}\right)+\frac{1}{2}\left(\frac{h^2}{4}\right)=\frac{h^2}{4}
\end{align*}
\tag{1.22}
$$
^122

Substituting [[#^120]] and [[#^122]] into [[#^121]], we can find that
$$
\begin{align*}
(\Delta S_z)^2=\frac{h^2}{4}-(0)^2=\frac{h^2}{4}\\
\Delta S_z=\sqrt{\frac{h^2}{4}}=\frac{h}{2}
\end{align*}
$$
for a particle in the state $\ket{+x}$.

We call $\Delta S_z$ the uncertainty rather than the standard deviation since a *single* particle in the state $\ket{+x}$ does not have a definite value for $S_z$.

## Spin State Predictions

$\braket{S_z}=0$ is not in disagreement with finding a single particle to be spin up if we measure $S_z$ on a particle in the state $\ket{+x}$.

To test predictions such as [[#^120]], we will need a statistically significant sample.

In general, if we make $N$ measurements, we should expect fluctuations that are on the order of $\sqrt{N}$.

Thus  with 100 measurements, deviations from $\braket{S_z}=0$ on the order of 10% is reasonable.

However, if we were to make $10^6$ measurements, and find 550,000 particles spin up and 450,000 particles spin down, then there is a problem.

We should expect fluctuations of only about $\sqrt{N}=1,000$ rather than the measured 50,000.

## Example 1.2

As in [[Stern-Gerlach Experiments#Example 1.1|Example 1.1]], a spin-$\frac{1}{2}$ particle is in the state
$$
\ket{\psi}=\frac{1}{2}\ket{+z}+\frac{i\sqrt{3}}{2}\ket{-z}
$$

What are the expectation value $\braket{S_z}$ and the uncertainty $\Delta S_z$ for this state?

---

The value of $\braket{S_z}$ is found by using equation [[#^120]]
$$
\braket{S_z}=c^*_+c_+\left(\frac{h}{2}\right)+c^*_-c_-\left(-\frac{h}{2}\right)
$$
where
$$
\begin{align*}
c^*_+c_+=\left|\braket{+z|\psi}\right|^2=\left(\frac{1}{2}\right)^2=\frac{1}{4}\\
c^*_-c_-=\left|\braket{-z|\psi}\right|^2=\left(\frac{i\sqrt{3}}{2}\right)^2=\left(\frac{-i\sqrt{3}}{2}\right)\left(\frac{i\sqrt{3}}{2}\right)=\frac{3}{4}
\end{align*}
$$

therefore substituting our values into [[#^120]] yields
$$
\begin{align*}
\braket{S_z}=\frac{1}{4}\left(\frac{h}{2}\right)+\frac{3}{4}\left(-\frac{h}{2}\right)\\
=\frac{h}{8}-\frac{3h}{8}=-\frac{2h}{8}=-\frac{h}{4}
\end{align*}
$$

To find the uncertainty $\Delta S_z$, we must first find the value of $\braket{S^2_z}$ using [[#^122]].
$$
\begin{align*}
\braket{S^2_z}=\frac{1}{4}\left(\frac{h}{2}\right)^2+\frac{3}{4}\left(-\frac{h}{2}\right)^2\\
=\frac{1}{4}\left(\frac{h^2}{4}\right)+\frac{3}{4}\left(\frac{h^2}{4}\right)^2\\
=\frac{h^2}{16}+\frac{3h^2}{16}=\frac{4h^2}{16}=\frac{h^2}{4}
\end{align*}
$$

Thus to find the expectation value $\Delta S_z$, we can substitute the values of $\braket S_z$ and $\braket{S^2_z}$ into [[#^121]].
$$
\begin{align*}
(\Delta S_z)^2=\braket{S^2_z}-\braket{S_z}^2=\frac{h^2}{4}-\frac{h^2}{16}=\frac{3h^2}{16}\\
\Delta S_z=\sqrt{\frac{3h^2}{16}}=\frac{\sqrt{3}}{4}h\approx0.43h
\end{align*}
$$

Thus the expectation value $\braket{S_z}=-h/4$ and the uncertainty $\Delta S_z=0.43h$ for the state $\ket{\psi}$.

> Note that the uncertainty $\Delta S_z$ is $0.43h$ which is a smaller value than $0.50h$ for the state $\ket{+x}$.

This reflects the fact that there is less uncertainty since there is a 75% probability of obtaining $h/2$ for $S_z$ for the state $\ket{\psi}$ compared to the 50% probability for the state $\ket{+x}$.

If the state of the particle were $\ket{+z}$, then there would be a 100% probability of obtaining $h/2$ for $S_z$, and $\Delta S_z=0$ .

# 1.5 Experiment 5

Replace the last SG$z$ device with one having its inhomogeneous magnetic field in the $y$ direction and make measurements of $S_y$.

Measure $S_y$ on particles exiting the SG$x$ in the state of $\ket{+x}$.

Since we're measuring $S_y$ instead of $S_z$, the percentage of particles going "up" and "down" remains the same as [[Stern-Gerlach Experiments#Experiment 3|Experiment 3]].

If we replaced the SG$x$ device with SG$y$ in Experiment 3, the results would be the same: 50% with $S_y=h/2$ and 50% with $S_y=-h/2$.

Same principle applies to replacing SG$z$ with SG$y$ with in Experiment 3: still 50% with $S_z=h/2$ and 50% with $S_z=-h/2$.

Measuring $S_y$ instead of $S_z$ shows that the direction of measurement doesn't affect the results, only the axis being measures on.

This reinforces the idea that measurements are observer-dependent, but the physical state of the system is independent of the measurement.

## Relative Phases

Just as we can express the state $\ket{+x}$ with [[#^118]], we can express the state $\ket{+y}$ as a superposition of $\ket{+z}$ and $\ket{-z}$ in the form
$$
\ket{+y}=\frac{e^{i\gamma_+}}{\sqrt{2}}\ket{+z}+\frac{e^{i\gamma_-}}{\sqrt{2}}\ket{-z}=\frac{e^{i\gamma_+}}{\sqrt{2}}\left[\ket{+z}+e^{i(\gamma_--\gamma_+)}\ket{-z}\right]
\tag{1.23}
$$
^123

where the complex numbers are written such that multiplying the kets $\ket{+z}$ and $\ket{-z}$ ensure that there is a 50% probability of obtaining $S_z=h/2$ and 50% probability of obtaining $S_z=-h/2$.

Note that the last step pulls out the overall phase factor $e^{i\gamma_+}$ for convenience.

![[PHYS375-Figure-1.9.png]]

Since there is a 50% chance of finding $S_y=h/2$ when it exits the SG$x$ device in the state $\ket{+x}$, we must have
$$
\left|\braket{+y|+x}\right|^2=\frac{1}{2}
\tag{1.24}
$$
^124

The bra corresponding to the ket [[#^123]] is
$$
\bra{+y}=\frac{e^{-i\gamma_+}}{\sqrt{2}}\bra{+z}+\frac{e^{-i\gamma_-}}{\sqrt{2}}\bra{-z}=\frac{e^{-i\gamma_+}}{\sqrt{2}}\left[\bra{+z}+e^{-i(\gamma_--\gamma_+)}\bra{-z}\right]
\tag{1.25}
$$
^125

where the complex numbers in [[#^123]] are replaced with their complex conjugates in going from [[#^123]] to [[#^125]].

Rewriting [[#^118]] by pulling out an overall phase factor yields:
$$
\ket{+x}=\frac{e^{i\delta_+}}{\sqrt{2}}\left[\ket{+z}+e^{i(\delta_--\delta_+)}\ket{-z}\right]
\tag{1.26}
$$
^126

then
$$
\begin{align*}
\braket{+y|+x}=\frac{e^{i(\delta_+-\gamma_+)}}{2}\left(\bra{+z}+e^{-i\gamma}\bra{-z}\right)\left(\ket{+z}+e^{i\delta}\ket{-z}\right)\\
=\frac{e^{i(\delta_+-\gamma_+)}}{2}\left[1+e^{i(\delta-\gamma)}\right]
\end{align*}
\tag{1.27}
$$
^127

where $\delta=\delta_-+\delta_+$ and $\gamma=\gamma_--\gamma_+$ are the **relative phases** between the kets $\ket{+z}$ and $\ket{-z}$ for these two states.

Furthermore, $\braket{+z|+z}=\braket{-z|-z}=1$ and $\braket{+z|-z}=\braket{-z|+z}=0$ is used to evaluate the amplitude.

We can now calculate the probability:
$$
\begin{align*}
\left|\braket{+y|+x}\right|^2=\left\{\frac{e^{i(\delta_+-\gamma_+)}}{2}\left[1+e^{i(\delta-\gamma)}\right]\right\}\left\{\frac{e^{i(\delta_+-\gamma_+)}}{2}\left[1+e^{i(\delta-\gamma)}\right]\right\}\\
=\frac{1}{4}\left[1+e^{i(\delta-\gamma)}\right]\left[1+e^{i(\delta-\gamma)}\right]\\
=\frac{1}{2}\left[1+\cos(\delta-\gamma)\right]
\end{align*}
\tag{1.28}
$$
^128

To agree with [[#^124]] requires $\delta-\gamma=\pm\pi/2$.
The common convention is to take $\delta=0$.

If in [[#^123]] and [[#^126]], we ignore the overall phases $\delta_+$ and $\gamma_+$, which appear in the amplitude [[#^127]] but do not enter into the calculation of the probability [[#^128]], we see that
$$
\ket{+x}=\frac{1}{\sqrt{2}}\ket{+z}+\frac{1}{\sqrt{2}}\ket{-z}
\tag{1.29}
$$
^129

and
$$
\ket{+y}=\frac{1}{\sqrt{2}}\ket{+z}+\frac{e^{i\pi/2}}{\sqrt{2}}\ket{-z}=\frac{1}{\sqrt{2}}\ket{+z}+\frac{i}{\sqrt{2}}\ket{-z}
\tag{1.30}
$$
^130

where $\gamma=\pi/2$.
The choice $\gamma=-\pi/2$ yields the state
$$
\frac{1}{\sqrt{2}}\ket{+z}-\frac{i}{\sqrt{2}}\ket{-z}=\ket{-y}
\tag{1.31}
$$
^131

![[PHYS375-Figure-1.10.png]]

There is an ambiguity because it was not specified if the coordinate system for the Stern-Gerlach experiments are left-handed or right-handed.

The state $\ket{+y}$ is the state with $S_y=h/2$ in a right-handed coordinate system, however $\ket{+y}$ is $S_y=-h/2$ in a left-handed coordinate system.

This is the reason why two solutions appear.

Furthermore, [[#^124]] cannot be explained without a complex amplitude.
The appearance of $i$ such as in [[#^130]] is a key ingredient of a description of nature by quantum mechanics. While classical physics use complex numbers as an aid for calculations, the Stern-Gerlach experiments *demand* complex numbers for their explanation.

## Example 1.3

A spin-$\frac{1}{2}$ particle is in the state
$$
\ket{\psi}=\frac{1}{2}\ket{+z}+\frac{i\sqrt{3}}{2}\ket{-z}
$$

What is the probability that a measurement of $S_y$ yields $h/2$? What is $\braket{S_y}$ for this state?

---

To calculate the probability that $S_y$ yields $h/2$, we can find the amplitude for $\braket{+y|\psi}$.

From [[#^130]] we can see that 
$$
\ket{+y}=\frac{1}{\sqrt{2}}\ket{+z}+\frac{i}{\sqrt{2}}\ket{-z}
$$
and to find the corresponding bra vector, we can replace each complex amplitude with their complex conjugates,
$$
\bra{+y}=\frac{1}{\sqrt{2}}\bra{+z}-\frac{i}{\sqrt{2}}\bra{-z}
$$
Now we can find the probability amplitude $\braket{+y|\psi}$,
$$
\begin{align*}
\braket{+y|\psi}=\left(\frac{1}{\sqrt{2}}\bra{+z}-\frac{i}{\sqrt{2}}\bra{-z}\right)\left(\frac{1}{2}\ket{+z}+\frac{i\sqrt{3}}{2}\ket{-z}\right)\\
=\left(\frac{1}{\sqrt{2}}\right)\left(\frac{1}{2}\right)\braket{+z|+z}+\left(-\frac{i}{\sqrt{2}}\right)\left(\frac{i\sqrt{3}}{2}\right)\braket{-z|-z}\\
=\frac{1}{2\sqrt{2}}+\frac{\sqrt{3}}{{2\sqrt{2}}}=\frac{1}{2\sqrt{2}}\left(1+\sqrt{3}\right)
\end{align*}
$$

Therefore the probability is
$$
\begin{align*}
\left|\braket{+y|\psi}\right|^2=\left|\frac{1}{2\sqrt{2}}(1+\sqrt{3})\right|^2=\left|\frac{1}{2\sqrt{2}}(1+\sqrt{3})\right|\left|\frac{1}{2\sqrt{2}}(1+\sqrt{3})\right|\\
=\left[\frac{1}{2\sqrt{2}}+\frac{\sqrt{3}}{2\sqrt{2}}\right]\left[\frac{1}{2\sqrt{2}}+\frac{\sqrt{3}}{2\sqrt{2}}\right]\\
=\frac{1}{8}+\frac{\sqrt{3}}{8}+\frac{\sqrt{3}}{8}+\frac{3}{8}=\frac{1}{2}+\frac{\sqrt{3}}{4}\approx0.93
\end{align*}
$$
The probability that a measurement of $S_y$ yields $h/2$ is 93%.

> To get a feel for what the spin state $\ket{\psi}$ is and why the probability of finding the particle in the state with $S_y=h/2$ is as large as 0.93, look at [[A Modern Approach to Quantum Mechanics by John S. Townsend.pdf#page=44&selection=5,0,34,70|Problem 1.10]]

To find the expectation value $\braket{S_y}$, we can use equation [[#^120]].
Since
$$
\begin{align*}
c^*_+c_+=\left|\braket{+y|\psi}\right|^2=\frac{1}{2}+\frac{\sqrt{3}}{4}\\
c^*_-c_-=\left|\braket{-y|\psi}\right|^2=1-\left|\braket{+y|\psi}\right|^2=1-\left(\frac{1}{2}-\frac{\sqrt{3}}{4}\right)=\frac{1}{2}-\frac{\sqrt{3}}{4}
\end{align*}
$$
it follows that,
$$
\begin{align*}
\\
\braket{S_y}=\left(\frac{1}{2}+\frac{\sqrt{3}}{4}\right)\left(\frac{h}{2}\right)+\left(\frac{1}{2}-\frac{\sqrt{3}}{4}\right)\left(-\frac{h}{2}\right)\\
=\left(\frac{h}{4}+\frac{\sqrt{3}h}{8}\right)+\left(\frac{-h}{4}+\frac{\sqrt{3}h}{8}\right)=\frac{\sqrt{3}h}{8}+\frac{\sqrt{3}h}{8}=\frac{\sqrt{3}}{4}h\\

\end{align*}
$$

> I would like to verify:
> $$
> \frac{\sqrt{3}h}{8}+\frac{\sqrt{3}h}{8}=\frac{\sqrt{3}}{4}h
> $$

Therefore, the expectation value $\braket{S_y}=(\sqrt{3}/4)h$.
