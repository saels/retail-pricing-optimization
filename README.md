# 🏷️ Retail Pricing Optimization

## 💼 Business use case

Pricing teams need more than a demand forecast. They need a decision rule that converts expected demand into executable prices while respecting price ladders, promotion limits, and merchandising policies. This project connects predictive demand logic with constrained optimization.

## 🎯 Principal objective

Optimize weekly revenue over weeks 157–169 using a demand equation driven by current price, lagged prices, and seasonal effects. The notebook builds four progressively more realistic Gurobi formulations, moving from unconstrained continuous prices to discrete price ladders and promotion rules.

## 🔎 Summary of takeaways

The project demonstrates an important production pattern: estimate demand first, then place an optimization layer on top of the prediction so that recommended actions satisfy real business constraints. The transition from continuous decisions to mixed-integer price-ladder models is what makes the formulation operationally relevant.

## 🧭 Explore the code

The [notebook](https://github.com/saels/retail-pricing-optimization/blob/184f2b8e9da820d36fee1ca87c47ed3286b74ad4/Retail_pricing_optimization.ipynb) is worth reviewing for the progression of optimization models and the way business policies are translated into mathematical constraints. The code shows how a pricing problem changes once recommendations must be executable, not merely theoretically optimal.
