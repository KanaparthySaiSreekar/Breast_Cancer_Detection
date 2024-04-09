We will tackle the problem of early breast cancer detection from X-ray images. Specifically, given a candidate region of interest (ROI) from an X-ray image of a patient's breast, the goal is to predict if the region corresponds to a malignant tumor (label 1) or is normal (label 0). The training and test data sets for this problem is provided in the file hw6_dataset.csv. Each row in these files corresponds to a ROI in a patient's X-ray, with columns 1-117 containing features computed using standard image processing algorithms. The last column contains the class label, and is based on a radiologist's opinion or a biopsy. This data was obtained from the KDD Cup 2008 challenge.

The data set contain a total of 69,098 candidate ROIs, of which only 409 are malignant, while the remaining are all normal.

The fitted model is better than all zeroes classifier because from its confusion matrix we can tell it can predict persons with cancer upto some extent rather than labeling everyone as non-cancer patient

Looking at only accuracy we can't tell that logistic regression is better than all zeroes classifier . but looking at confusion matrix proves this wrong.. hence in this condition where there is severe imbalance for judging which is better

If we look at

Accuracy for fitted classifier 0.9955707582335658
Accuracy for all zeros classifier 0.9946059728983029
Accuracy for fitted classifier is only a little better than the all zeros classifier.

Therefore we look at the confustion matrix to see the score results.

Confusion Matrix for fitted classifier
[[22670    10]
 [   91    32]]
Confusion Matrix for all 0's classifier
[[22680     0]
 [  123     0]]
