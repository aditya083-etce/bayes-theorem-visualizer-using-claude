# Bayes' Theorem Chalkboard

An interactive, chalkboard-styled visualization of Bayes' theorem applied to diagnostic testing — explore how sensitivity, specificity, and prevalence affect the reliability of a positive test result.

## Files

- `index.html` — page markup and logic
- `styles.css` — chalkboard styling (fonts, colors, hand-drawn effects)

Keep both files in the same folder — `index.html` links to `styles.css` via a relative path.

## Usage

Open `index.html` in any browser. No build step or server required.

## Features

- **Sliders** for Sensitivity, Specificity, and Prevalence (1–100%)
- **Dynamic bar graph** showing True Positive / False Positive / False Negative / True Negative probabilities, recalculated live
- **2×2 outcome matrix** (TP, FN, FP, TN)
- **Bayes' theorem equation** displayed in chalk-style fraction notation
- **PPV callout** explaining, in plain language, what fraction of positive results are true positives at the current settings

## Formula

```
P(Cov|+) = [P(+|Cov) · P(Cov)] / [P(+|Cov) · P(Cov) + P(+|DF) · P(DF)]
```

Where `Cov` = condition present, `DF` = disease-free, `+` = positive test result.