---
tags:
  - quantum-mechanics
---

# 2.1 The Beginnings of Matrix Mechanics

## Representing Kets and Bras

We can represent a ket $\ket{\psi}$ by a column vector
```math
\ket{\psi}\underset{S_z\;\mathsf{basis}}{\longrightarrow}
\begin{pmatrix}
	\braket{+z|\psi} \\ \braket{-z|\psi}
\end{pmatrix}
=
\begin{pmatrix}
	c_+ \\ c_-
\end{pmatrix}
```

In this basis, the ket $\ket{+z}$ is represented by the column vector
```math
\ket{+z}\underset{S_z\;\mathsf{basis}}{\longrightarrow}\begin{pmatrix}
	\braket{+z|+z} \\ \braket{-z|+z}
\end{pmatrix}
=
\begin{pmatrix}
	1 \\ 0
\end{pmatrix}
```

and the ket $\ket{-z}$ is represented by
```math
\ket{-z}\underset{S_z\;\mathsf{basis}}{\longrightarrow}\begin{pmatrix}
	\braket{+z|-z} \\ \braket{-z|-z}
\end{pmatrix}
=
\begin{pmatrix}
	0 \\ 1
\end{pmatrix}
```

We can also represent (1.29) as
```math
\ket{+x}\underset{S_z\mathsf{basis}}{\longrightarrow}\begin{pmatrix}
	\braket{+z|+x} \\ \braket{+z|-x}
\end{pmatrix}
=
\begin{pmatrix}
	1/\sqrt{2} \\ 1/\sqrt{2}
\end{pmatrix}
=\frac{1}{\sqrt{2}}
\begin{pmatrix}
	1 \\ 1
\end{pmatrix}
```

(1.30) indicates that the state $S_y=h/2$ is
```math
\ket{+y}\rightarrow \frac{1}{\sqrt{2}}\begin{pmatrix}
	1 \\ i
\end{pmatrix}
```

The bra corresponding to the ket is represented in the same basis by
```math
\bra{+y}=\frac{1}{\sqrt{2}}\begin{pmatrix}
	1 & -i
\end{pmatrix}
```

## Example 2.1

Use matrix mechanics to determine the probability that a measurement of $S_y$ yields $h/2$ for a spin-$\frac{1}{2}$ particle in the state
```math
\ket{\psi}=\frac{1}{2}\ket{+z}+\frac{i\sqrt{3}}{2}\ket{-z}
```

```math
\begin{align*}
\braket{+y|\psi}=\frac{1}{2}\braket{+y|+z}+\frac{i\sqrt3}{2}\braket{+y|-z}\\
=\frac{1}{2}\begin{pmatrix}
	1 & i
\end{pmatrix}\begin{pmatrix}
	1\\
0
\end{pmatrix}+\frac{i\sqrt{3}}{2}\begin{pmatrix}
	1 & i
\end{pmatrix}\begin{pmatrix}
	0\\
1
\end{pmatrix}
\end{align*}
```

#todo Complete example 2.1

## 2.2

## 2.3

## 2.4

## 2.5

## 2.6

