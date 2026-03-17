---
exports:
  - format: pdf
    template: lapreprint-typst
    id: pdf-export
downloads:
  - id: pdf-export
    title: Download PDF
---
# Energy Demand

+++ {"part": "abstract"}
What is the energy demand of a building? This chapter explores different approaches to calculating or estimating the energy demand of a building, ranging from simple ballpark estimations to complex, detailed simulations.
+++

## 1. Ballpark Estimations

What is the simplest way to get a ballpark number and when would one attempt a simulation?

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

> "To understand the universe, you must understand energy, frequency, and vibration." — [Nikola Tesla](https://en.wikipedia.org/wiki/Nikola_Tesla)

Here is a summary table of different methods:

| Method | Accuracy | Complexity |
| --- | --- | --- |
| Rules of Thumb | Low | Very Low |
| Steady-State | Medium | Low |
| Dynamic Simulation | High | High |

## 2. Simulations: Levels of Complexity

If simulation is the goal, what are the different levels of complexity?

### R51C Models

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur vel tortor ut tellus convallis accumsan. Integer quis egestas sem, eu ullamcorper dui.

The equation for the R51C network can be simplified as $Q = \frac{\Delta T}{R}$.

$$
C \frac{dT}{dt} = \frac{T_{ext} - T}{R} + Q_{internal}
$$

### Energy Balance Models

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam erat volutpat. Phasellus vel nisi non odio egestas rhoncus. Suspendisse potenti.

Here is an example code snippet that sets up a simple energy balance calculation:

```python
def calculate_energy_balance(T_in, T_out, R_value, Area):
    """
    Calculates the heat loss through a surface.
    """
    delta_T = T_in - T_out
    U_value = 1 / R_value
    heat_loss = U_value * Area * delta_T
    return heat_loss

# Example usage
loss = calculate_energy_balance(20, -5, 3.0, 50)
print(f"Heat Loss: {loss} W")
```

### Neural Networks & Machine Learning

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent commodo cursus magna, vel scelerisque nisl consectetur et. Nullam id dolor id nibh ultricies vehicula ut id elit.

![An abstract representation of a neural network](https://picsum.photos/seed/neural/800/400)
*Figure 1: Conceptual visualization of interconnected data.*
