# CancerDetection
# 1. Project Topic and Goal
This project is about developing an algorithm to identify metastatic cancer in small image patches extracted from larger digital pathology scans. The dataset used for this competition is a modified version of the PatchCamelyon (PCam) benchmark dataset, which focuses on the detection of metastasis in cancer patients.

# 2. Data
The dataset consists of many small pathology images for classification. Each image has an image id, and the train_labels.csv file offers the true labels for images in the train folder. The objective is to predict labels for images in the test folder. Positive labels indicate the presence of tumor tissue in the central 32x32px section of a patch (with tumor tissue in the surrounding area not affecting the label). This outer region supports fully-convolutional models that maintain consistency when applied to whole-slide images, without zero-padding.

Train and test data combined exhibit a size of rougly 7.76 GB which is quite large. There are 220,000 training train images and 57,000 test images, each represented in a .tif format. For evaluation we are required to create a submission file consisting of a 2-column table. First, there will be the ID of the test images and second the predicted label (1 = positive, 0 = negative).

# 3. Solution
Solution is provided in jupyter notebook file.
