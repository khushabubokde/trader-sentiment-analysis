# Trader Sentiment Analysis

This project analyzes the relationship between Bitcoin market sentiment (Fear/Greed index) and trader behavior and performance using Hyperliquid trade data.

## Motivation

Traders often react emotionally to market conditions. This project explores how sentiment (like Fear or Greed) affects trading decisions and performance.

## Installed Packages

The following Python libraries were used in this project:

```bash
pip install pandas
pip install numpy
pip install matplotlib
pip install seaborn
pip install scikit-learn
pip install jupyter

## Data Used

- **Fear & Greed Index**
  - Daily sentiment scores
- **Hyperliquid Trade Data**
  - Order execution, PnL, trade side, timestamps, etc.

Include where the data came from and how it was cleaned/processed.

## How to Run

```bash
git clone https://github.com/khushabubokde/trader-sentiment-analysis
cd trader-sentiment-analysis
pip install -r requirements.txt
jupyter notebook trader-sentiment-analysis.ipynb

```markdown
## Methodology

1. Load and clean both datasets
2. Merge trader and sentiment data by date
3. Compute daily metrics
4. Compare performance under Fear vs Greed

## Key Insights

- Traders trade more aggressively in Greed
- PnL volatility increases under Greed
- Strong sentiment extremes show distinct trader behavior

This gives real context to what your analysis shows — just like other sentiment analysis repos do.

## Future Improvements

- Build an interactive dashboard
- Add machine learning prediction models
- Compare with other sentiment sources like news or Twitter

## Trading Strategy

Based on the analysis of Fear & Greed sentiment data and trader performance, the following strategy is proposed:

1.Sentiment-Based Positioning

- **Extreme Fear**
  - Market is oversold
  - Opportunity to take LONG positions
  - Historically better risk-reward

- **Fear**
  - Trade cautiously
  - Smaller position sizes

- **Neutral**
  - Market consolidation phase
  - Range-based strategies preferred

- **Greed / Extreme Greed**
  - Market may be overbought
  - Consider SHORT positions
  - Reduce exposure and protect profits

 2.Risk Management Rules

- Use stop-loss for every trade
- Avoid high leverage during Extreme Greed
- Reduce trade frequency during high volatility periods
- Monitor win rate by sentiment classification

 3. Data-Driven Insight

Analysis shows that:
- PnL distribution changes significantly across sentiment classes
- Win rate varies between Fear and Greed periods
- Trader behavior becomes aggressive in Greed phases

This strategy leverages sentiment cycles to improve entry timing and risk control.


