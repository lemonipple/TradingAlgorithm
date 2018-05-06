# TradingAlgorithm

Problem Statement

What market conditions such as liquidity or volatility are relevant when determining which type of execution algorithm (VWAP, IS, Dark) to use?

Each execution algo follows some benchmark. The benchmark may be price, in which case you end up with IS. Or it may be actual traded quantity, in which case you end up with POV. Or it may be historical traded quantity, in which case you end up with VWAP. Or it may be time, in which case you end up with TWAP. Or it may be a million other things.

The algo will constanly be querying how it is doing agaist the benchmark. If it is ahead of the benchmark, it will use some of it to try to improve on something else - usually price. If it is falling behind the benchmark, it will compromise on what it can (usually price) in order to catch up.

There is no execution algo called “Dark”. “Dark Pool” is a type of trading venue - one that does not publish the contents of its order books. Most algos are agnostic to the venue, and they will typically use all available venues.



TWAP VWAP

VWAP can be used as a metric to gauge a trader's competency and reward performance. Those who short above the vwap or buy below the vwap and close profitably are rewarded. Fundamentally, VWAP is the average price paid per share

With TWAP, say the price trades in a very narrow range for a long time but the volume is very light. 
