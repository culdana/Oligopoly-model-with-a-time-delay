# Discrete Cournot Oligopoly Model with Delay and Memory (Mathematica)

This repository contains the implementation of a dynamic Cournot oligopoly model in Mathematica. The model includes a delay mechanism where firms partially react to past decisions.

## Description

Each firm in the oligopoly updates its production based on:
- a reaction to its own previous output,
- the average outputs of all firms after a fixed delay,
- a delay weight parameter δ (delta) that balances current and past influence.

The dynamics are explored through bifurcation diagrams and Lyapunov exponents as δ varies.

## Key Features

- Evolution function using `Max[]` to constrain output to non-negative values
- Memory effects modeled through discrete delays
- Automatic generation of bifurcation diagrams
- Lyapunov exponent analysis

## Files

- `main_code.m`: Main Mathematica script
- `README.md`: Documentation

## Usage

1. Open `main_code.m` in Wolfram Mathematica.
2. Define parameters:
   - `nfirme` – number of firms
   - `T` – delay length
   - `a1`, `be` – constants
3. Run the script to visualize the behavior of the system as δ ∈ [0, 1].

## Output

- Bifurcation diagram of the first firm’s output vs. δ
- Lyapunov exponent plot (optional, not plotted in code)

## License

MIT License
