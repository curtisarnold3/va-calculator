# VA Disability Pay Estimator

A free, single-page tool that estimates how a veteran's monthly VA disability pay could change if a rating goes up or a new condition is added. Uses the VA combined-ratings math (38 CFR 4.25) and bilateral factor (38 CFR 4.26) with published 2026 rates.

**Not affiliated with the U.S. Department of Veterans Affairs. Estimate only; the VA makes the final decision.**

Live: https://curtisarnold3.github.io/va-calculator/
Demo with sample data: https://curtisarnold3.github.io/va-calculator/?demo=1

## Files

- `index.html` – the whole app (HTML, CSS, JS inline). No build step, no dependencies.
- `test.js` – checks the combined-ratings math.

## Run the tests

```bash
node test.js
```

Prints one line per case and exits non-zero on any failure.
