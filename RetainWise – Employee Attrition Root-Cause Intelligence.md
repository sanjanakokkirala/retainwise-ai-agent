# RetainWise

Employee attrition root-cause intelligence · Demo company: Infosys-style IT services firm · 500 synthetic employees, ₹ lakh

## 1 · What drives attrition (learned by the model)

Bars show the model’s learned effect of each factor. Red raises attrition risk, green lowers it. Each bar is a one-standard-deviation change.

## 2 · Where the problem is concentrated

## 3 · Retention interventions ranked by return

Each intervention is simulated on the current employees: the model re-scores them after the change, and savings = leavers avoided × replacement cost (1.5× annual salary).

## 4 · Highest-priority at-risk employees

## 5 · RetainWise AI agent

## How it works (algorithm)

1\) Integrate HRIS, performance, payroll, attendance, overtime, engagement survey and training data → 2) Engineer features (compa-ratio, overtime, absenteeism, engagement, training hours, tenure, performance, time since promotion) → 3) Train an attrition model (logistic regression here; gradient boosting + SHAP or survival analysis in production) → 4) Rank drivers by learned effect → 5) Find hotspots by department and the main driver in each → 6) Simulate interventions on current employees and compute savings against cost → 7) Recommend evidence-based actions and re-train quarterly. Correlation is not proof of cause, so pilot interventions and measure them.