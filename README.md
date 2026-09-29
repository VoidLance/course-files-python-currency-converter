# Python Currency Converter

A small Python command-line program that converts a USD amount to euros (EUR), British pounds (GBP), and Japanese yen (JPY) using configured exchange rates.

## Features

- Converts one USD amount to EUR, GBP, and JPY.
- Keeps each conversion available as a Python function for reuse.
- Uses local, configurable exchange-rate constants; no third-party packages are required.

## Getting started

### Requirements

Python 3.6 or later is required. The program also imports an `exchange_rates.py` module, which is not included in this repository. Create that file in the same directory as `currency_converter.py` and define the three rates:

```python
# Example rates only. Replace these with current rates for your use.
USD_TO_EUR = 0.92
USD_TO_GBP = 0.79
USD_TO_JPY = 150.0
```

The values above are illustrative and are not updated automatically.

### Run the converter

From the project directory, run:

```bash
python currency_converter.py
```

Enter an amount in USD when prompted. For example, with the illustrative rates above, entering `100` prints the corresponding amounts in EUR, GBP, and JPY.

### Use the conversion functions

You can also import the functions into another Python program:

```python
from currency_converter import convert_usd_to_eur, convert_usd_to_gbp, convert_usd_to_jpy

print(convert_usd_to_eur(100))
print(convert_usd_to_gbp(100))
print(convert_usd_to_jpy(100))
```

## Help

For questions or to report a problem, [open an issue](https://github.com/VoidLance/course-files-python-currency-converter/issues).

## Maintainers and contributions

No individual maintainer or separate contribution guide is specified in this repository. Contributions are welcome through GitHub issues and pull requests. Please keep changes focused and describe how you tested them.
