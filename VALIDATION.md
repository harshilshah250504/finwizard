# Validation notes

## Model smoke check — 19 September 2026

The CNN, SimpleRNN and LSTM constructors from the final notebook experiment were imported without executing its downloads or long training loops. Each model completed one training batch and produced finite predictions of shape `(8, 1)` from synthetic inputs of shape `(8, 60, 1)`.

Environment: Python 3.12, TensorFlow 2.21, Keras 3.15.1.

This checks model compatibility and basic execution only. It is not a reproduction of paper metrics or evidence of trading performance. News API integration requires a separately configured credential.

## Evaluation limitations

The historical notebook includes exploratory variants. In the final experiment, scaling is fitted before the train/test split and predictions are aligned to a month by slicing rather than explicit dates. A reliable backtest must fit preprocessing on training data only, align predictions by date, use chronological validation and compare against a naive baseline. Existing metric comments should not be treated as independently verified results.
