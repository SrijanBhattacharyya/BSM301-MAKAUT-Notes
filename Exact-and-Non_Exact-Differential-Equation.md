# General Form
```txt
f(x, y) =    dy/dx   = - (M(x, y)/N(x, y))
        => Mdx + Ndy = 0
```


# Exact Differential Equation
## Criteria for Exactness
* The necessary and sufficient condition for `Mdx + Ndy = 0` to be exact is:
  ```txt
   𝛿M     𝛿N
  ---- = ----
   𝛿y     𝛿x
  ```

## Ways to Solve Exact Differential Equation
   * <details>
      <summary>Way 1</summary>

   **Equation:** `Mdx + Ndy = 0`
   
   ### Steps to solve:
   1. ∫Mdx                        `[y is constant]`
   2. ∫Ndy                        `[x is constant]`
   3. Add the results of the above steps.

   > **NOTE:**
   <br> Don't repeate anything during the addition.
   </details>
   * <details>
      <summary>Way 2</summary>

   **Equation:** `Mdx + Ndy = 0`
   
   ### Steps to solve:
   1. ∫Mdx                        `[y is constant]`
   2. ∫ndy                        `[n are the terms of N without x as their coefficient]`
   3. Add the results of the above steps.
   </details>


# Non-Exact Differential Equations
## Criteria for Non-Exact Differential Equation
* The necessary and sufficient condition for `Mdx + Ndy = 0` to be exact is:
  ```txt
   𝛿M     𝛿N
  ---- ≠ ----
   𝛿y     𝛿x
  ```

## Integrating Factor (If)
### Definition
    Differential Equations which are not exact differential equation, can be made exact differential equation by multiplying it with a switable factor sometimes. The switable factor may be a function of `x` or `y` or both. The switable factor is called the **Integrating Factor** of the equation.

### How to find the Integrating Factor of an Equation
   1. ```python
      if ((𝛿M/𝛿y) - (𝛿N/𝛿x))/N == f(x):
          If = e**(∫f(x)dx)
      ```
   2. ```python
      if ((𝛿N/𝛿x) - (𝛿M/𝛿y))/N == g(y):
          If = e**(∫f(y)dy)
      ```

## Ways to Solve Non-Exact Differential Equation
1. Multiply the equation with it's Integrating Factor.
2. Now it has become an Exact Differential Equation.
3. Solve it in [this way](https://github.com/SrijanBhattacharyya/BSM301-MAKAUT-Notes/blob/main/Exact-and-Non_Exact-Differential-Equation.md#ways-to-solve-exact-differential-equation).
