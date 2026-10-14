# spotify-machine-learning-project

Music streaming platforms like Spotify have transformed how people consume music, making it vital for artists, record labels, and marketing teams to understand what drives track popularity. This project addresses the core business question: "Which audio and metadata characteristics best predict a song's streaming success on Spotify?"

## Comparative Performance and Final Model Choice

The Master Evolution Summary reports test RMSE and test R² for all seven models on the same log_streams test set. From the table and plots, the pattern is:
Baseline Linear Regression: Achieves a strong starting performance on the log scale, with relatively low test RMSE and high test R², showing that linear relationships already capture a substantial portion of the variance in log-streams.
Regularised Linear Models: The Ridge, Lasso, and ElasticNet models provide performance very similar to the baseline, with small changes in test RMSE and test R², but with added stability due to regularisation.
Gradient Boosting Models: Show a clear improvement, especially after tuning:
  GBR (Untuned): Shows a reduction in test RMSE compared with the linear family.
  GBR (Tuned Round 1): Further improves performance.
  GBR (Tuned Round 2 / Final): Achieves the lowest test RMSE and one of the highest test R² values      among all seven models.

Based on these results, we selected "GBR (Tuned Round 2 / Final)" as the final model, because it offers the best trade-off between low prediction error (RMSE) and high explained variance (R²), under a consistent evaluation framework.

## Business Interpretation

From a business perspective, the final Gradient Boosting model can be used to forecast expected streaming performance of tracks based on their metadata, exposure, and audio characteristics. For example, the model can help identify high-potential tracks (predicted high log-streams but currently low exposure) and support decisions on where to focus marketing and playlisting efforts.


