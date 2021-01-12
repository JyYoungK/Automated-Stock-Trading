# Stock
 
Buy signal as soon as the price manages to break out.
After buying the security we'll want to send out a trading stop loss
As soon as it drops more than a certain amount the position will be closed.
The idea behind this trading stop-loss is to cut our losers short and let the winners run.
Unlike humans an algorith can't just use its judgment to determine which level is the best therefore we have to specify how a breakout is defined for
our strategy to work.
The easiest approach for this would be to say we look at the closing prices for the last three months and whatever price is the highest is our breakout level.
Why 3 months? If volatility is high we want to look further into the past than when volatility is relatively low. By doing this the algorithm will automatically adapt to changes in volatility.
The strategy that we're going to implement is a simple breakout strategy that dynamically changes its lookback length furthermore it uses a trading stop loss to protect against potential losses.
