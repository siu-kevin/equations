---
title: Moisture Codes
summary: FFMC, DMC, DC
order: 2
---

### FFMC
\[ \texttt{mo} = \texttt{mo} + \texttt{rf} \cdot \texttt{rain} \cdot \exp\bigg(\frac{-100}{251 - \texttt{lastmc}}\bigg) \cdot \Bigg(1 - \exp\bigg(\frac{-6.93}{\texttt{rain}}\bigg)\Bigg) \]