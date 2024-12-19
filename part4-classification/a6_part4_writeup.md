# Part 4 - Classification Writeup

After completing `a6_part4.py` answer the following questions

## Questions to answer

1. Comment out the StandardScaler and re-run your test. How accurate is the model? Why is that?
Without standardization, the model's accuracy may decrease because logistic regression is sensitive to the scale of the features. Features with larger ranges can dominate the optimization process, leading to suboptimal performance.
2. How accurate is the model with the StandardScaler? Is this model accurate enough for the given use case? Explain.
Using the Standard Scaler, the model performs with approximately 85% accuracy, which exceeds expectations. However, despite testing with smaller sample sizes, there remains a notable likelihood of incorrect predictions.
3. Looking at the predicted and actual results, how did the model do? Was there a pattern to the inputs that the model was incorrect about?

Although standardized data points around zero appear to improve accuracy, a clear correlation for incorrect predictions isn't easily identified just by observing individual cases. Without visualizing these incorrect predictions in bulk, it's difficult to draw a data-driven conclusion.

4. Would a 34 year old Female who makes 56000 a year buy an SUV according to the model? Remember to scale the data before running it through the model.

It predicted that she would not purchase an SUV.