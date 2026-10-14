# Micevski Adnex Notation (`adnex.sty`)

Official LaTeX package introducing the **Adnex operator** ($\adnex$) for algebraic concatenation, designed by Petar Micevski.

## Overview

In traditional mathematics, there is no standardized operator for concatenating digits or evaluated expressions directly into a single positional number without explicitly writing scaling operations like $100 \cdot N + k$. 

The **Adnex package** introduces two notation forms for mathematical concatenation along with a dedicated digit variable:

1. **Digit Variable ($\zeta_{\text{I}}$):** Represents a single digit constraint ($1 \le \zeta_{\text{I}} \le 9$).
2. **Linear Adnex ($\adnex$):** Concatenates a single scalar or calculated digit to the end of a value.
3. **Wave Adnex ($\wadnex{\dots}$):** Concatenates an entire evaluated algebraic expression or function under a curved vinculum.

---

## Example: Formula for Squaring Numbers Ending in 5

Using the Micevski Adnex notation, the mental trick for squaring any number ending in 5 (e.g., $35^2 = 1225$) is expressed concisely as:

$$\zeta_{\text{I}} \cdot (\zeta_{\text{I}} + 1) \adnex 25$$

---

## Installation & Usage

1. Download `adnex.sty` and place it in your LaTeX project directory.
2. Add `\usepackage{adnex}` to your LaTeX document preamble.

### Commands

| Command | Output | Description |
| :--- | :--- | :--- |
| `\zetaone` | $\zeta_{\text{I}}$ | Single-digit variable (Zeta-One) |
| `\adnex` | $\adnex$ | Linear Adnex operator for single values |
| `\wadnex{expr}` | $\wadnex{expr}$ | Wave Adnex operator for grouped expressions |
