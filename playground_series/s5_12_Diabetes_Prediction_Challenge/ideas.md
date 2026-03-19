📘 1. Regression Algorithms in scikit-learn (sklearn)
🔹 Linear Models

LinearRegression — Ordinary Least Squares (OLS)

Ridge / RidgeCV

Lasso / LassoCV

ElasticNet / ElasticNetCV

Lars, LassoLars

OrthogonalMatchingPursuit (OMP)

BayesianRidge

ARDRegression (Automatic Relevance Determination)

HuberRegressor

RANSACRegressor (robust regression)

TheilSenRegressor

PoissonRegressor

GammaRegressor

TweedieRegressor

SGDRegressor (stochastic gradient descent)

QuantileRegressor

🔹 Polynomial / Basis Function Regression

PolynomialFeatures + LinearRegression

SplineTransformer + LinearRegression

🔹 Tree-based and Ensemble Regression

DecisionTreeRegressor

RandomForestRegressor

ExtraTreesRegressor

GradientBoostingRegressor

HistGradientBoostingRegressor

AdaBoostRegressor

BaggingRegressor

IsolationForest (not regression, anomaly detection—but often grouped under ensemble)

🔹 Support Vector Regression

SVR

LinearSVR

NuSVR

🔹 Nearest Neighbor Regression

KNeighborsRegressor

RadiusNeighborsRegressor

🔹 Neural Network Regression

MLPRegressor

🔹 Gaussian Process Regression

GaussianProcessRegressor

🔹 Isotonic / Nonparametric Regression

IsotonicRegression

KernelRidge

LocalOutlierFactor (not regression, but kernel methods nearby)

📗 2. Regression Tools in scipy.stats

scipy.stats is mainly for statistical distributions — it does not include full regression APIs like sklearn or statsmodels.

The only true regression-related tools are:

🔹 Least-squares Regression

scipy.stats.linregress — simple OLS for two variables (univariate linear regression)

🔹 Curve Fitting (Nonlinear Regression)

scipy.optimize.curve_fit — nonlinear least-squares fitting

scipy.optimize.least_squares — general-purpose nonlinear regression

🔹 Orthogonal Distance Regression (errors in both x & y)

scipy.odr.ODR

scipy.odr.Model, scipy.odr.RealData

📙 3. Regression Models in statsmodels

statsmodels is the closest to R and provides the richest set of statistical regression models.

🔹 Linear Regression (Classical)

OLS — Ordinary Least Squares

GLS — Generalized Least Squares

WLS — Weighted Least Squares

GLSAR — GLS with AR errors

🔹 Generalized Linear Models (GLM)

GLM with families:

Gaussian

Binomial (Logistic Regression)

Poisson

Gamma

Tweedie

Negative Binomial

🔹 Robust Regression

RLM — Robust Linear Models (Huber, Tukey, Hampel, etc.)

🔹 Discrete Regression

Logit

Probit

Poisson

NegativeBinomialP

MNLogit (multinomial logit)

🔹 Time Series Regression

SARIMAX — seasonal ARIMA + exogenous regressors

ARIMA

ARMA

AR / AutoReg

VAR — vector autoregression

VARMAX — VAR with moving average

UnobservedComponents (structural models)

StateSpace models

🔹 Nonlinear and Mixed Models

MixedLM — linear mixed-effects models (random effects)

QuantReg — quantile regression

NLS — nonlinear least squares

GEE — generalized estimating equations