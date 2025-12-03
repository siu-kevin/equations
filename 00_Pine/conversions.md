---
title: Conversions
summary: Moisture Code to Moisture Content (%)
order: 1
---

Functions to convert FWI moisture codes FFMC, DMC, and DC to their corresponding moisture contents (%).

### FFMC to mcffmc
$$ \texttt{mcffmc} = \frac{14875 \cdot (101 - \texttt{ffmc})}{101 \cdot (59.5 + \texttt{ffmc})} $$

### mcffmc to FFMC
$$ \texttt{ffmc} = \frac{59.5 \cdot (250 - \texttt{mcffmc})}{\frac{14875}{101} + \texttt{mcffmc}} $$

### DMC to mcdmc
$$ \texttt{mcdmc} = \frac{280}{\exp(\frac{\texttt{dmc}}{43.43})} + 20 $$

### mcdmc to DMC
$$ \texttt{dmc} = 43.43 \cdot \ln\bigg(\frac{280}{\texttt{mcdmc} - 20}\bigg) $$

### DC to mcdc
$$ \texttt{mcdc} = 400 \cdot \exp\bigg(-\frac{\texttt{dc}}{400}\bigg) $$

### mcdc to DC
$$ \texttt{dc} = 400 \cdot \ln\bigg(\frac{400}{\texttt{mcdc}}\bigg) $$
