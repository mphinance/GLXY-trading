# GLXY Trade Alerts — Entry/Breakout/BTC Momentum

This Pine Script indicator is designed for the TradingView platform to provide visual and alert-based signals for trading GLXY, based on a combination of price action, volume, and Bitcoin (BTC) momentum.

## Features

* **Entry Zone:** A user-defined price range where the indicator will signal a potential entry opportunity if a bullish candle and rising Relative Strength Index (RSI) are present.

* **Breakout Zone:** A user-defined price range above which the indicator will signal a potential breakout. This signal is filtered by a volume multiplier to confirm strength.

* **Structural Stop:** A critical support level where a break below can trigger an alert, suggesting a potential exit.

* **BTC Momentum:** The script checks for a significant daily percentage change in BTC to provide an additional layer of confirmation for breakout signals.

* **Visuals:** The indicator plots horizontal lines for key levels and uses shaded zones to clearly highlight the Entry and Breakout zones on the chart. Upward and downward facing labels mark entry and breakout signals.

## User Inputs

* `Entry Zone Low`: The lower bound of the entry zone.

* `Entry Zone High`: The upper bound of the entry zone.

* `Breakout Zone Low`: The lower bound of the breakout zone.

* `Breakout Zone High`: The upper bound of the breakout zone.

* `Structural Stop`: The price level for the structural stop.

* `Volume Avg Length`: The length of the moving average used to calculate average volume.

* `Volume Multiplier`: The multiplier used to confirm a breakout signal with volume.

* `BTC Symbol`: The symbol for BTC used for momentum checks (e.g., `BINANCE:BTCUSD`).

* `BTC daily % threshold to consider momentum`: The percentage change in BTC required to trigger the momentum confirmation.

## Alerts

The script includes several `alertcondition`s that can be used to set up automated alerts on TradingView.

* **GLXY Entry Zone Signal:** Triggers when a valid entry signal is found within the entry zone.

* **GLXY Breakout:** Triggers when the price breaks into the breakout zone with sufficient volume.

* **GLXY Breakout + BTC Momentum:** Triggers when the price breaks out with volume, and there is a significant positive BTC momentum.

* **GLXY Structural Stop Hit:** Triggers when the price falls below the structural stop level.

To set up an alert, right-click on the chart, select "Add Alert," and choose the corresponding alert condition from the dropdown menu.
