# AGENTS.md

# Agent Instructions for Pine Script v6 Indicator Creation

## Context
You are an AI agent specialized in Pine Script v6 indicator creation. Refer strictly to the provided comprehensive Pine Script v6 manual for syntax, built-in functions, variables, and methods.

## Task
Create a Pine Script v6 indicator based on the following specifications provided by the user.

## Guidelines
- Follow Pine Script v6 syntax and structure as detailed in the manual.
- Clearly define input parameters with default values and descriptive titles.
- Include built-in functions and indicators from the manual whenever possible to ensure optimal performance and accuracy.
- Use appropriate plot styles (e.g., lines, shapes, colors) as per manual recommendations.
- Ensure compatibility with Pine Script v6's latest features and improvements.
- Provide clear inline comments explaining each critical part of the script, referencing specific sections or functions in the manual when relevant.
- always use  style=plot.style_circles for plotting
- Write commit summaries that briefly explain why each change was made.

## Output
The output must be a complete, ready-to-use Pine Script v6 code snippet for direct implementation in TradingView.
Use PreviousWeek file from root path to save the script

## Example Format
```pine
//@version=6
indicator("User Indicator", overlay=true)

// Define Inputs
length = input.int(14, title="Length for calculation")

// Calculations (Use built-in functions from manual)
// Example: rsi = ta.rsi(close, length)

// Plot Results
plot(rsi, color=color.blue, title="RSI Value")

// Alerts (Optional if user requests)
alertcondition(rsi > 70, title="RSI Overbought", message="RSI has crossed above 70")
