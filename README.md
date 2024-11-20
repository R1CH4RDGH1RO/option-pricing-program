# Option Pricing Program

## Overview
The **Option Pricing Program** calculates the prices of European and American call and put options for a stock based on user inputs. It uses the following models:

- **European Options**: Black-Scholes model.
- **American Options**: Binomial model with the CRR Exact Solution approach for up and down factor determination.

## Features
- Supports pricing of:
  - European Call and Put Options
  - American Call and Put Options
    
- Incorporates user-defined inputs such as:
  - Stock price
  - Strike price
  - Time to expiration
  - Risk-free interest rate
  - Dividend yield
  - Volatility
    
- Provides robust input validation.

## Installation
1. Clone the repository:
   ```bash
   git clone <https://github.com/R1CH4RDGH1RO/option-pricing-program.git>
   ```
2. Navigate to the directory:
   ```bash
   cd <repository-folder>
   ```
3. Ensure you have Python 3 installed. The program requires the `math` module, which is part of the Python standard library.

## Usage
1. Run the program:
   ```bash
   python Option_Pricing_Program.py
   ```
2. Enter the required inputs as prompted


| Variable Name | Description                                                      |
|---------------|------------------------------------------------------------------|
| `S`           | Current stock price                                             |
| `K`           | Option strike price                                             |
| `T`           | Time to expiration (in years)                                   |
| `r`           | Risk-free interest rate (e.g., 0.03 for 3%)                     |
| `y`           | Dividend yield rate (e.g., 0.02 for 2%)                         |
| `sigma`       | Volatility of the underlying stock (e.g., 0.25 for 25%)         |
| `option_type` | Type of option: `E` for European, `A` for American              |
| `call_put`    | Type of option: `C` for Call, `P` for Put                       |
| `u`           | Up factor in the Binomial model                                 |
| `d`           | Down factor in the Binomial model                               |
| `p`           | Risk-neutral probability in the Binomial model                 |

3. The program calculates and displays the option price based on your inputs.

## Example
Sample execution:
```
Enter current stock price: 100
Enter option strike price: 95
Enter time to expiration (in years): 0.5
Enter risk-free interest rate: 0.03
Enter dividend yield: 0.02
Enter volatility: 0.25
Enter the option type, E = European, A = American: E
Enter the option type, C = Call, P = Put: C
European Call Option Price: 6.2048
```

## Limitations
- Assumes constant volatility and interest rates.
- Models may not capture extreme market conditions.

## License
This project is licensed under the [MIT License](LICENSE).

## Contributions
Feel free to submit issues or create pull requests for bug fixes or feature enhancements.

---

### Contact
For further information or questions, please contact me on [LinkedIn](www.linkedin.com/in/riccardo-mingolla).
