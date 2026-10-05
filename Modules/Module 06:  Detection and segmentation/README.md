# Lab 06: Object Detection and Image Segmentation
ITAI 1378 Computer Vision

### Overview

In this lab, you will use modern computer vision tools to detect and segment objects in images. You will run YOLO11 for object detection, YOLO11-seg for instance segmentation, compare specialist models with foundation models such as SAM 2, and begin planning your midterm project.

By the end of this lab, you should be able to explain the difference between classification, detection, and segmentation; run an object detector and read its output; create and interpret segmentation masks; compare YOLO and SAM 2; explain IoU, precision, recall, and mAP in plain English; and propose a midterm project idea using concepts from Modules 1 to 6.

Estimated time: 2 to 3 hours

What You Need
You will need:

A free Google account
Google Colab
The notebook: ipynb
Internet access
Optional: one or two images of your own to test
You do not need a GPU, prior YOLO or Ultralytics experience, or advanced math.

Setup
Open Google Colab, sign in, and upload the provided notebook. Run the notebook from top to bottom using Shift + Enter. The first cell installs Ultralytics and may take a minute or two. If Colab disconnects, reconnect and rerun the cells from the beginning. Do not leave the lab unfinished overnight without saving your work.

Lab Tasks
Complete each notebook section in order.

Sections 1 to 3: Read the introduction and concepts comparing classification, detection, and segmentation. Run the setup and sample image cells.

Section 4: Run YOLO11 object detection on the sample image. You should see bounding boxes around detected objects.

Your Turn 1: Run detection on a different image, either from another Ultralytics sample URL or an image you upload to Colab.

Confidence Threshold Experiment: Run the comparison using different confidence thresholds and observe how detections change.

Section 5: Run YOLO11-seg for instance segmentation and compare the masks to the bounding boxes.

Your Turn 2: Run segmentation on the same custom image used in Your Turn 1 and evaluate whether the masks are accurate.

Section 6: Run the YOLO plus SAM 2 detect-then-segment pipeline. Remember that SAM 2 creates masks but does not provide category labels.

Section 7: Read the evaluation concepts and run the IoU visualization cell.

Section 8: Review the midterm project examples and choose or design a project direction.

Section 9: Answer all ten reflection questions. You may write your answers in markdown cells inside the notebook (preferred) or in a separate document. Question 10 must include a focused midterm project pitch paragraph. Keep responses focused and specific, usually two to four sentences per question.

Required Submissions
Submit your work in Canvas before the due date listed in the syllabus. Your reflection answers can live inside the notebook or in a separate file, so you will submit either one file or two depending on the option you choose.

Completed Notebook (required)
All cells must be run from top to bottom.
Sections: Your Turn 1 and Your Turn 2 must use an image different from the sample image.
The notebook should run without errors.
Outputs must be visible. Do not clear them before submitting.
Reflection Answers (required, choose one option)
Preferred: answer all ten questions in markdown cells inside the notebook. If you do this, the notebook is your only file and there is nothing else to submit for the reflection.
Alternative: answer all ten questions in a separate document and submit it as a PDF.
Either way, Question 10 must include a focused midterm project pitch paragraph.
File Naming Convention
Use this exact format with your real HCC enrollment name. Use underscores only and do not use spaces in file names.

Notebook: ipynb
Separate reflection, only if you chose the PDF option: pdf
Grading
Total: 100 points

Implementation and Exercises: 60 points
Section 4 detection demo: 10 points
Your Turn 1 detection on your own image: 10 points
Confidence threshold experiment: 10 points
Section 5 segmentation: 10 points
Your Turn 2 segmentation on your own image: 10 points
Section 6 SAM 2 detect-then-segment pipeline: 10 points
Reflection: 40 points
Each reflection question is worth 4 points:

Classification vs. detection vs. segmentation
Non-Maximum Suppression
What IoU measures
Your own image detection analysis
When to use boxes vs. masks
SAM 2 versus YOLO labeling
Confidence threshold trade-off
Precision vs. recall scenarios
Specialist vs. foundation model
Midterm project pitch
Bonus Opportunities
You may earn up to 10 bonus points maximum:

Try a larger YOLO11 variant and compare results: +3
Run YOLO-World for open-vocabulary detection: +3
Write a short comparison of SAM 2 and SAM 3: +2
Fine-tune YOLO11 on a small custom dataset: +5
How This Lab Is Graded
Code: Functionally correct code earns full credit. Points are not deducted for cell placement, combining steps, or code style as long as the code runs and produces visible output.

Results: Imperfect detections or masks that are honestly reported and analyzed are not penalized. If masks look messy, that is useful material for the reflection, not an automatic failure.

Reflection: Answers may be written in markdown cells inside the notebook (preferred) or in a separate PDF. Full credit means the answer is specific, correct, and addresses the question in two to four sentences.

Part A: Implementation and Exercises (60 points)
Criterion

Points

What earns full credit

Section 4 detection demo

10

YOLO11 runs on the sample image; bounding boxes and the printed detection summary are visible.

Your Turn 1: detection on your own image

10

Detection runs on an image different from the sample, and the result is shown and briefly judged.

Confidence threshold experiment

10

Detection is run at the different thresholds and the change in number of detections is visible.

Section 5 segmentation

10

YOLO11-seg runs; the masks are displayed and a single mask is shown on its own.

Your Turn 2: segmentation on your own image

10

Segmentation runs on the same custom image and the mask quality is judged.

Section 6 SAM 2 detect-then-segment

10

SAM 2 runs using the YOLO11 boxes as prompts and the resulting masks are displayed.

Part A subtotal

60

 

Part B: Reflection (40 points)
Each of the ten questions is worth 4 points.

Criterion

Points

What earns full credit

1. Classification vs. detection vs. segmentation

4

Distinguishes the three tasks with a workforce example of each.

2. Non-Maximum Suppression

4

Explains what NMS does and why YOLO uses it.

3. What IoU measures

4

Describes overlap quality in plain English.

4. Your own image detection analysis

4

Reflects on what the model got right or wrong on the student's image.

5. When to use boxes vs. masks

4

Gives one case for a box and one case for a mask.

6. SAM 2 versus YOLO labeling

4

Explains why SAM 2 producing no labels matters.

7. Confidence threshold trade-off

4

Gives a low-threshold and a high-threshold application with reasons.

8. Precision vs. recall scenarios

4

Chooses correctly for a safety system and a photo tagger, with reasons.

9. Specialist vs. foundation model

4

Explains when to reach for YOLO11-seg versus SAM 2.

10. Midterm project pitch

4

One paragraph covering what it does, the data source, and a capstone extension.

Part B subtotal

40

 

Bonus (up to 10 points maximum)
Bonus items are added after the 100 base points, capped at 10 total even though the items below sum to more.

Criterion

Points

What earns full credit

Larger YOLO11 variant compared

+3

Runs a larger YOLO11 variant and compares results to the nano model.

YOLO-World open-vocabulary detection

+3

Runs open-vocabulary detection with a text-described class.

SAM 2 versus SAM 3 comparison

+2

Short written comparison of what SAM 3 adds over SAM 2.

Fine-tune YOLO11 on a small custom dataset

+5

Fine-tunes YOLO11 on a small custom dataset and reports the outcome.

Total: 100 points, plus up to 10 bonus
