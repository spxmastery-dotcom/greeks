# greeks
SPX Options Greeks Analyzer

Copywrite: SPXMASTERY.com  Russell Clark Sept 8, 2025.  All rights are reserved.  No use of this website or contents may be used without the expressed written permission of the author.

SPX Nov 28 7000 Call: Interactive Greeks Analyzer

This repository hosts a single-page web application for visualizing and analyzing the Greeks (Delta, Gamma, Theta, Vega) of 10 SPX Nov 28, 2025, 7000 Call options contracts. Built with HTML, CSS, JavaScript, and Chart.js, it provides real-time calculations and charts based on user inputs.

Features
Input Parameters: Adjust SPX price, days to expiration, implied volatility (IV), and risk-free rate to update calculations.

Greeks Table: Displays Greeks for Current, Breakeven, 20% Profit, and High Profit scenarios, with color-coded rows (yellow for current, green for profit).

Interactive Charts: Plots Delta, Gamma, Theta, and Vega across SPX 6400-7100, with red/yellow/green thresholds for actionable insights.

Black-Scholes Model: Calculates option price and Greeks, matching provided data (e.g., Delta ~90.24, Gamma ~0.52, Theta ~-362, Vega ~4877 at SPX 6499).

Usage
Visit https://spxmastery.github.io/greeks.

Enter values (e.g., SPX=6499, Days=81, IV=10.21%, RF=4%).

Click "Update Table & Charts" to populate the table and render charts.

Review:

Table: Check Delta (>100 green), Gamma (>0.6 green), Theta (>-400 green), Vega (>5000 green).

Charts: Blue lines show Greek values; dashed red/yellow/green lines indicate exit/wary/profit zones.

Notes: Breakeven ~6508; Vega gains ~$975 per 0.2% IV increase; exit if SPX <6480.

Technical Details
File: index.html (self-contained with embedded CSS/JS).

Dependencies: Chart.js (loaded via CDN: https://cdn.jsdelivr.net/npm/chart.js).

Model: Black-Scholes for option pricing and Greeks, using 252 trading days for Theta.

Hosting: GitHub Pages, accessible at https://spxmastery.github.io/greeks.

FINRA-Compliant Disclaimer: Risks of Options Trading
Options trading involves significant risks and is not suitable for all investors. The SPX Nov 28 7000 Call Interactive Greeks Analyzer is provided solely for educational and informational purposes to illustrate the theoretical behavior of options Greeks (Delta, Gamma, Theta, Vega) using the Black-Scholes model. It is not intended as financial, investment, or trading advice, nor as a recommendation to buy, sell, or hold any securities, including SPX options or any other financial instruments.

High Risk of Loss: Options trading carries a high risk of substantial financial losses, potentially exceeding the initial investment. The value of options can decline rapidly due to factors such as market volatility, time decay (Theta), changes in the underlying asset (SPX), and other economic or market conditions. Losses can be magnified for leveraged positions, such as the 10 contracts modeled in this tool.

No Guarantee of Accuracy: The calculations and visualizations provided (e.g., Delta ~90.24, Theta ~-362 at SPX 6499) are based on theoretical models (Black-Scholes) and user inputs (SPX price, IV, etc.). Actual market conditions, pricing, and outcomes may differ significantly due to factors like bid-ask spreads, liquidity, transaction costs, or model limitations. The tool does not account for taxes, commissions, or other fees.

User Responsibility: Any use of this tool, including entering custom inputs (e.g., SPX=6499, IV=10.21%) or interpreting outputs (charts, tables), is at the user’s sole risk. The creator of this tool (spxmastery) expressly disclaims any responsibility or liability for any financial losses, damages, or consequences resulting from decisions made based on the tool’s outputs or information.

Not Professional Advice: This tool is not a substitute for professional financial advice. Users should consult a qualified financial advisor, broker, or other professional before engaging in options trading or any investment activities. The creator is not a registered investment advisor, broker, or financial professional.

Market Risks: Options on the S&P 500 Index (SPX) are subject to market risks, including sudden price movements, volatility spikes, or macroeconomic events. The tool’s thresholds (e.g., Delta >100 green, Theta >-400 green) are illustrative and not prescriptive; actual trading outcomes depend on individual strategies and market conditions.

Educational Use Only: The tool is designed to help users understand options Greeks and their theoretical behavior. It does not provide real-time market data, and users must verify inputs (e.g., current SPX price, IV) independently. The tool is not intended for use in live trading or investment decision-making.

No Warranty: The tool is provided “as is” without warranties of any kind, express or implied, including accuracy, reliability, or fitness for a particular purpose. Technical issues (e.g., charts not rendering) may occur; check the console (F12) for errors like “Chart.js not loaded.”

Regulatory Compliance: Options trading is regulated by the Financial Industry Regulatory Authority (FINRA) and the Securities and Exchange Commission (SEC). Users must comply with all applicable laws and regulations. For more information on options risks, refer to the Options Disclosure Document (ODD) provided by the Options Clearing Corporation.

By using this tool, you acknowledge that you understand the risks of options trading and agree that the creator (spxmastery) is not liable for any financial losses or damages incurred. Always conduct thorough research and seek professional advice before trading options.

Notes
As of Sep 8, 2025. Not financial advice—use for educational visualization.

If charts fail, check console (F12) for errors (e.g., "Chart.js not loaded").

Update inputs for real-time market data.

Setup
Clone or fork this repository: https://github.com/spxmastery/greeks.

Ensure index.html is in the greeks folder of the spxmastery.github.io repository.

GitHub Pages is enabled for the main branch, serving the site at https://spxmastery.github.io/greeks.

To update, edit index.html or README.md and commit changes.
