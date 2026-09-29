# Risk Scoring Program

## About the Project

This is a simple Python program made to calculate a risk score using three different factors. The factors used in this program are inflation, border tension, and resource scarcity.

The user gives a value from 1 to 10 for each factor. The program then uses different weights for each factor and calculates a final Threat Index out of 100.

I made this project to understand how weighted values and basic decision-making can be used in a Python program.

## Factors Used

The program takes these three inputs:

1. **Inflation Level** - value from 1 to 10
2. **Border Tension Level** - value from 1 to 10
3. **Resource Scarcity Level** - value from 1 to 10

Here, 1 means low risk and 10 means very high risk.

## Weights

Different importance is given to each factor:

- Inflation = 0.20
- Border Tension = 0.30
- Resource Scarcity = 0.50

Resource scarcity has the highest weight in this model.

## Formula

The weighted score is calculated using:

`(Inflation × 0.20) + (Tension × 0.30) + (Scarcity × 0.50)`

After that, the result is multiplied by 10 to get the Threat Index out of 100.

## Risk Levels

- **75 or above:** High Risk
- **45 to below 75:** Moderate Risk
- **Below 45:** Low Risk

## Example

If the user enters:

- Inflation = 6
- Border Tension = 7
- Resource Scarcity = 8

The calculation is:

`(6 × 0.20) + (7 × 0.30) + (8 × 0.50) = 7.3`

So the Threat Index is:

`7.3 × 10 = 73.0`

The program will show **Moderate Risk**.

## How to Run

1. Install Python on your computer.
2. Save the program as a `.py` file.
3. Open the terminal or command prompt in that folder.
4. Run:

```bash
python risk_scoring.py
```

5. Enter the three values when the program asks for them.

## Technologies Used

- Python
- Basic variables
- User input
- Arithmetic calculations
- If-elif-else conditions

## Note

This is a simple academic project made to demonstrate weighted scoring in Python. The Threat Index is only based on the values entered by the user and should not be considered an actual prediction of real-world conflict or risk.
