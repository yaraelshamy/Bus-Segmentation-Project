# SBEN424-Advanced-CV-Final Project
## By: 
* Ahmed Helmy Ahmed          ID: 1170539
* Salma Hazem Abdallah       ID: 1170425
* Yara Wael Mohamed          ID: 1170431

# What's it all about?
## Image Segmentation:
### Our approach in BUS images for lesion segmentation

<table>
  <thead>
    <tr>
      <th>Input</th>
      <th>Preprocessing</th>
      <th>Segmentation</th>
      <th>Postprocessing</th>
      <th>Output</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Gray Scale Image</td>
      <td>Histogram Equalization(optional)</td>
      <td> Quick Shift</td>
      <td>Normalization</td>
      <td>Binary Image</td>
    </tr>
    <tr>
      <td></td>
      <td>Inverting </td>
      <td></td>
      <td>Clear Boarder</td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>Edge Enhancement </td>
      <td></td>
      <td>Region with Largest Area</td>
      <td></td>
    </tr>
    <tr>
      <td></td>
      <td>Median</td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
  </tbody>
</table>


## Evaluation Metrics:
We compared our implemented model to the given model using a variety of metrics.<br>

**Metrics used:**
* True Positive   
* True Negative
* False Positive
* False Negative
* False Negative rate
* Sensitivity
* Specificity
* Accuracy
* Dice Coefficient
* Jaccard Index
* Precision Recall Curve


# How can you use our code?

* run all functions in **(Helper Functions)** section
* in **Get best threshold (training)** section or in **./results/QS-EDGE-MEDIAN-UDIAT/threshold accuracy.txt**  you can see the accuracy of all thresholds 
* Check that the **GT** and **Input** folders are included within the data folder.
* If not add them or change the paths of the variables *img_array & gt_array*.
* main script is last script in main.ipynb **(Main script)**
* Then simply run the main script.
* Within the results folder, you will see a folder named **QS-EDGE-MEDIAN-UDIAT**, which contains all of the output images from each step as well as the final output.
* You will also get a text file named **results.txt** in **QS-EDGE-MEDIAN-UDIAT**, which has a table with all of the image evaluation metrics, as well as their averages and standard deviation.
