# NTO_2_team
Hello, this is my first repo to store our handwriting recognition solution.
This is a solution for the task of the NTO Olympiad in the profiles of Artificial Intelligence.
I had several hypotheses, some of them were complete nonsense, and some of them were useful.


1)First I made a loss function based on the CLIP, I quickly realized that this was a very bad idea for this task

2)Then we decided to build a model based on Attention. This gave a good quality, but soon after the end of the Olympiad, we realized that the best model was based on CRNN + CTC loss

3)As word segmentation, detectron2 was used, and the model was called mask_rcnn_R_50_C4_1x, plus the average image resolution gave a quality of about 0.87 by F1 score
