# Engineering Mathematics: Terminal Velocity of a Falling Object

## Problem
How does the velocity of an object change as it falls through air?

## Modeling (Newton’s Second Law)
Forces acting on the object:
* **Gravity**: $mg$
* **Air resistance (drag)**: $cv$

Thus, the differential equation is:
$$m \frac{dv}{dt} = mg - cv$$

## Solving the Differential Equation

### 1. Rewrite
$$\frac{dv}{dt} = g - \frac{c}{m}v$$

### 2. Separate Variables
$$\frac{dv}{g - \frac{c}{m}v} = dt$$

### 3. Integrate
$$-\frac{m}{c} \ln\left(g - \frac{c}{m}v\right) = t + C$$

### 4. Rearrange
$$g - \frac{c}{m}v = Ae^{-\frac{c}{m}t}$$

### 5. Solve for $v(t)$
$$v(t) = \frac{mg}{c}(1 - Ae^{-\frac{c}{m}t})$$

### 6. Initial Condition
Assuming $v(0) = 0 \implies A = 1$

## Final Answer
$$v(t) = \frac{mg}{c}\left(1 - e^{-\frac{c}{m}t}\right)$$

## Physical Interpretation
* As $t \to \infty$, velocity approaches terminal velocity: $v_{terminal} = \frac{mg}{c}$
* The object initially accelerates.
* Acceleration decreases over time as air resistance increases.
* Eventually, the object reaches a constant speed (Terminal Velocity).
