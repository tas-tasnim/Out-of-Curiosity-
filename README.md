# Out of Curiosity

Small programs I write just to understand how something works.

## Number Base Converter (`Numbers_convertion.py`)

This program converts numbers between bases (decimal ↔ binary, octal, etc.) and **prints every step of the working**, the same way you'd do it by hand in a digital-logic class:

- **Decimal → any base:** repeated division, showing each quotient and remainder, then reading the remainders from LSD to MSD.
- **Any base → decimal:** positional expansion (`digit × base^power`).

```
$ python Numbers_convertion.py
Please enter your number, base and base of converted number (ex: 15 10 8): 15 10 2
15/2 = 7 --> 1
7/2 = 3 --> 1
3/2 = 1 --> 1
1/2 = 0 --> 1

LSD -- > MSD
the result is :  1111
```

**Planned:** support for bases above 10 (hex digits A–F), and fixing the exponent shown in the step-by-step expansion.
