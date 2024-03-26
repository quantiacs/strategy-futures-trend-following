# Futures Trend based strategy

This trading strategy is designed for the [Quantiacs](https://quantiacs.com/contest) platform, which hosts competitions
for trading algorithms. Detailed information about the competitions is available on
the [official Quantiacs website](https://quantiacs.com/contest).

## How to Run the Strategy

### In an Online Environment

The strategy can be executed in an online environment using Jupiter or JupiterLab on
the [Quantiacs personal dashboard](https://quantiacs.com/personalpage/homepage). To do this, clone the template in your
personal account.

### In a Local Environment

To run the strategy locally, you need to install the [Quantiacs Toolbox](https://github.com/quantiacs/toolbox).

## Strategy Overview

This Jupyter notebook, titled `strategy.ipynb`, outlines a **trend-following** trading strategy focusing on **futures
markets**. The strategy progresses from a simple, **single-pass implementation** to a more sophisticated **multi-pass
version**. It utilizes the `xarray` library for handling **multidimensional datasets**, making extensive use of labels
such as "time", "field", and "asset". This approach is particularly well-suited for **financial data analysis**.

**Technical analysis indicators** like the **Weighted Moving Average (WMA)** and the **Rate of Change Percentage (
ROCP)** are leveraged to discern market trends. Initially, the strategy is applied to **single assets**, then scaled
to **multiple assets** using a single-pass approach for efficiency and a multi-pass approach for **comprehensive
backtesting**.

The notebook includes comprehensive code snippets for **data loading**, **indicator calculation**, **trading signal
definition**, and **result visualization** with libraries such as **Plotly**. It integrates **Quantiacs**
libraries (`qnt`) for tasks such as **data loading**, **statistical analysis**, **graphical representation**, and 
**technical analysis**. The strategy highlights the criticality of choosing suitable **parameters** and **assets** to
optimize performance.
