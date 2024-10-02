# Positive-Volatility
Positive Volatility w/Volume Gauge in Pine Script

Overview:
This PineScript creates an indicator called the Positive Volatility and Volume Gauge with True Momentum Oscillator. It's designed to help traders visualize volatility, volume, and momentum in a clear way.

Key Features:
Version: Built using Pine Script version 5.
Separate Pane: The indicator is displayed in a separate area below the main price chart.

Input Parameters:
ATR Length: Sets the number of periods for calculating the Average True Range (default: 14).
Signal Threshold: Multiplier used for the upper signal line (default: 1.5).
Momentum Length: Determines the number of periods for calculating momentum (default: 14).
Oversold Level: Sets the threshold for oversold conditions (default: -1).
Overbought Level: Sets the threshold for overbought conditions (default: 1).

Calculations:
Real Volatility: Measures the market's true range using the ta.tr() function.
Positive Volatility: Filters out any negative values, showing only positive volatility.
Upper Signal Line: Calculated as a simple moving average (SMA) of positive volatility, adjusted by the signal threshold.
Volume Gauge: Normalizes the volume by dividing it by 25,000 for better visualization.
True Momentum Oscillator: Measures momentum based on the closing prices using the ta.mom() function.

Visual Representation:
Positive Volatility: Shown as a blue line.
Upper Signal Line: Represented as an orange line.
Volume Gauge: Displayed as a yellow histogram for easy interpretation.
True Momentum Oscillator: Plotted as a green line with:
Oversold Level: Indicated by a red horizontal line.
Overbought Level: Indicated by a green horizontal line.

Purpose:
This indicator provides traders with insights into market conditions by highlighting volatility, volume, and momentum, helping them make informed trading decisions.
