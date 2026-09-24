## Lab 05 - Chihuahua or Muffin Workshop Instructions

**Step 1: Set Up the Environment**

Option A: Google Colab

Open Google Colab:
1. Go to [Google Colab](https://colab.research.google.com/).
2. Sign in with your Google account if prompted.

Open the Notebook from GitHub:
1. Click on `File` > `Open notebook`.
2. Select the `GitHub` tab.
3. Enter the repository URL or your GitHub username and repository name: `patitimoner/workshop-chihuahua-vs-muffin`.
4. Select the `CNN_1 Chihuahua or Muffin.ipynb file to open

Clone the Entire Repository in Colab:
1. In the first cell of the notebook, add the following commands to clone the repository and ensure the data files are available:
   ```python
   !git clone https://github.com/patitimoner/workshop-chihuahua-vs-muffin.git
   %cd workshop-chihuahua-vs-muffin
   !ls
   ```

2. Press `Shift + Enter` to run the cell.

Option B: Amazon SageMaker Studio Lab

Open Amazon SageMaker Studio Lab:
1. Go to [Amazon SageMaker Studio Lab](https://studiolab.sagemaker.aws/).
2. Sign in with your Amazon account or create a new one if you don't have an account.

Clone the Repository:
1. Open a new terminal in SageMaker Studio Lab.
2. Run the following command to clone the repository:
   ```bash
   git clone https://github.com/patitimoner/workshop-chihuahua-vs-muffin.git
   ```

Navigate to the Cloned Directory:
1. Change the directory to the cloned repository:
   ```bash
   cd workshop-chihuahua-vs-muffin
   ```

Open the Notebook:
1. In the SageMaker Studio Lab file browser, navigate to the `workshop-chihuahua-vs-muffin` directory.
2. Open the notebook `CNN_1 Chihuahua or Muffin.ipynb`.

**Step 2: Modify the Code (if necessary)**

1. Review the Code:
   - Ensure all necessary imports are present at the beginning of the notebook and you have replaced the "?"  with the  correct code

 

**Step 3: Run the Notebook**

1. Execute Cells:
   - Run each cell of the notebook in order, carefully reading the outputs and checking for any errors.

2. **Handle Errors:**
   - If you encounter any errors, review the error message, check your code, and consult the course materials or ask for help if needed.

**Step 4: Experiment and Analyze**

1. Experiment with the Model:
   - Try different configurations to see how they affect the model’s performance:
     - Adjust the number of epochs.
     - Modify the learning rate.
     - Change the model architecture (e.g., add or remove layers).

2. Analyze Results:
   - For each experiment, note the changes in model performance.

**Step 5: Write Your Reflective Journal**

Write a 2-page reflective journal about your experience with this CNN-based classification task. Include the following:

1. CNN Architecture:
   - Briefly describe the CNN architecture and how it differs from the traditional neural network used in the previous workshop.

2. Model Performance:
   - Observe and report on the model's performance, including accuracy and any interesting patterns in the misclassifications.

3. Comparison:
   - Compare the CNN with the traditional neural network model in terms of performance and training time.

4. **Challenges and Solutions:**
   - Reflect on the challenges you faced during the lab and how you overcame them.

5. Real-World Applications:
   - Consider potential real-world applications of this type of image classification model.

6. Ethical Considerations:
   - Discuss any ethical considerations regarding the development and deployment of such models.

   Support your reflections with references to course materials or external sources on deep learning and computer vision.
