# Apple Stock Price Prediction Analysis
## LSTM & Reinforcement Learning Trading System

### Overview
This project integrates deep learning and reinforcement learning to automate stock trading for Apple Inc. (AAPL). It uses an LSTM model to forecast price movements and a DQN-based agent to execute trades.

### Technical Implementation
- **Data Source**: AAPL Historical Data (1980–2020).
- **Window Size**: 50 days of lookback.
- **Normalization**: MinMaxScaler (0,1).
- **Model**: Keras-based LSTM for time-series forecasting.
- **Agent**: Reinforcement Learning agent with Epsilon-Greedy exploration and Experience Replay.

### Trading Logic
The agent observes the market state (composed of normalized price data) and chooses one of three actions:
1. **Hold**: No change in position.
2. **Buy**: Open a long position.
3. **Sell**: Close position/take profit.

### Results Summary
- **Test Profit**: $151.31
- **Activity**: 700 Buy signals vs. 52 Sell signals in the test set.
- **Assessment**: The model shows a learning trend across 25 training episodes, with significant profit growth in later stages.

### Risk Metrics
- **Equity Curve**: Monitored for steady growth.
- **Max Drawdown**: Calculated to assess the potential for losses during market volatility.