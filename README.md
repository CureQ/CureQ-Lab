<!-- CureQ logo -->
<a href="https://cureq.github.io/CureQ/">
    <img src="./images/CureQ_logo.jpg" alt="MEAlytics logo" width=200px>
</a>

# CureQ-Lab
This repository contains [libraries for the CureQ consortium](#cureq-projects) and [research projects of the AUAS CureQ Lab](#other-auas-projects), which are developed as part of the Applied Artificial Intelligence (AI) master thesis and the Biomedical Engineering (BMT) bachelor thesis at the Amsterdam University of Applied Sciences (HvA).

## CureQ projects

We have made <i>2</i> GUI's for projects regarding the CureQ consortium. 
1. The [MEAlytics GUI](#mealytics) performs analysis of the Micro-electrode Array (MEA) experiments.
2. The [Microscopy GUI](#microscopy) performs analysis of microscopy images.<br><br>

---

<br> 

<a href="https://cureq.github.io/CureQ/">
    <img src="./images/MEAlytics_logo.ico" alt="MEAlytics logo" width=100px>
</a>

### MEAlytics

[MEAlytics](https://github.com/CureQ/CureQ) is a python package for analyzing Micro-electrode Array (MEA) experiments. This package offers high speed spike, burst and network burst detection followed by feature extraction. <br>The whole analysis tool is implemented in a Graphical User Interface (GUI). This GUI is used to inspect the raw MEA data and the analysis results. A few examples about the spike detection, burst detection and feature extraction can be found below &darr;

<!-- MEAlytics images -->
<!-- Table Image styling for multiple images near eachother -->
<table>
  <tr>
    <td align="center" width=50%>
      <a href="https://cureq.github.io/CureQ/view_results">
        <img src="./images/MEAlytics_spike_detection.png" alt="MEAlytics - Spike Detection"/>
      </a>
      <br/>
      <sub>MEAlytics - Spike Detection</sub>
    </td>
    <td align="center" width=50%>
      <a href="https://cureq.github.io/CureQ/view_results">
        <img src="./images/MEAlytics_network_burst_detection.png" alt="MEAlytics - Network Burst Detection">
      </a>
      <br/>
      <sub>MEAlytics - Network Burst Detection</sub>
    </td>
  </tr>
</table>

<table>
  <tr>
    <td align="center" width=50%>
      <a href="https://cureq.github.io/CureQ/compare_groups">
        <img src="./images/MEAlytics_group_comparison.png" alt="MEAlytics - Group Comparison">
      </a>
      <br/>
      <sub>MEAlytics - Group Comparison</sub>
    </td>
    <td align="center" width=50%>
      <a href="https://cureq.github.io/CureQ/compare_groups">
        <img src="./images/MEAlytics_features_over_time.png" alt="MEAlytics - Features over Time">
      </a>
      <br/>
      <sub>MEAlytics - Features over Time</sub>
    </td>
  </tr>
</table>

The MEAlytics tool also has a few other extensions (branches), which has not yet been merged with the main branch. These projects are about a newly introduced [Synchronisation method](#synchronisation) and a [Spike heatmap & Machine Learning predictions](#spike-heatmap--machine-learning-predictions).

---

### Synchronisation

An extra feature for the MEAlytics tool is about [Synchronisation](https://github.com/CureQ/CureQ/tree/Luca_synchronisation) methods. Synchrony is the degree of connectivity between two electrodes based on how synchronized the activity is across these electrodes. Synchrony differs from the already existing <i>network bursts</i> feature from the MEAlytics tool, because the <i>network bursts</i> feature requires at least half of the electrodes in a well to be active and the network burst detection is often delayed or absent because of this strict requirement. 

A spike train is a sequence of all detected spikes from an electrode. Examples of two spike trains and the Inter Spike Interval between these two spike trains can be found in the images below &darr;

<!-- Synchrony explanation images -->
<!-- Table Image styling for multiple images near eachother -->
<table>
  <tr>
    <td align="center" width=50%>
      <a href="https://github.com/CureQ/CureQ/tree/Luca_synchronisation">
        <img src="./images/Synchrony_Spike_trains.png" alt="Synchronicity - Synthetic Spike trains">
      </a>
      <br/>
      <sub>Synchronicity - Synthetic Spike trains</sub>
    </td>
    <td align="center" width=50%>
      <a href="https://github.com/CureQ/CureQ/tree/Luca_synchronisation">
        <img src="./images/Synchrony_ISI_over_time.png" alt="Synchronicity - ISI graph over time">
      </a>
      <br/>
      <sub>Synchronicity - ISI over time</sub>
    </td>
  </tr>
</table>

---

### Spike heatmap & Machine Learning predictions

An other project for the MEAlytics tool consisted of the 2 features: [Spike heatmap & Machine Learning predictions](https://github.com/CureQ/CureQ/tree/Lucas). 

1. The [Spike heatmap frame](https://github.com/CureQ/CureQ/blob/Lucas/docs/heatmap.md) generates an animation of a well overview heatmap with the activity of each electrode. It is also possible to show a heatmap showing the total activity of each electrode, and a heatmap showing the maximum per second activity of each electrode.

<!-- Heatmap images -->
<!-- Table Image styling for multiple images near eachother -->
<table>
  <tr>
    <td align="center" width=50%>
      <a href="https://github.com/CureQ/CureQ/blob/Lucas/docs/heatmap.md">
        <img src="./images/Heatmap.png" alt="Heatmap animation - Activity of each electrode">
      </a>
      <br/>
      <sub>Heatmap animation - Activity of each electrode</sub>
    </td>
    <td align="center" width=50%>
      <a href="https://github.com/CureQ/CureQ/blob/Lucas/docs/heatmap.md">
        <img src="./images/Heatmap_Total_Activity.png" alt="Heatmap - Total activity of each electrode">
      </a>
      <br/>
      <sub>Heatmap - Total activity of each electrode</sub>
    </td>
  </tr>
</table>

<br>

2. There is also a second added frame in this branch, which is about the [Machine Learning predictions](https://github.com/CureQ/CureQ/tree/Lucas).

<!-- Microscopy images -->
<!-- Table Image styling for multiple images near eachother -->
<table>
  <tr>
    <td align="center" width=50%>
      <a href="https://github.com/CureQ/CureQ/tree/Lucas">
        <img src="./images/ML_Frame_Labels.png" alt="Machine Learning Frame and label picker">
      </a>
      <br/>
      <sub>Machine Learning Frame</sub>
    </td>
    <td align="center" width=50%>
      <a href="https://github.com/CureQ/CureQ/tree/Lucas">
        <img src="./images/ML_Performances.png" alt="Performance Random Forest ML model">
      </a>
      <br/>
      <sub>Machine Learning Performances</sub>
    </td>
  </tr>
</table>

---

### Microscopy 

The [Microscopy GUI](https://github.com/CureQ/Microscopy) performs segmentation and statistical calculations on microscopy images. <br>The current main version provides the cell body detection application to analyze microscopy images and identify cell bodies in the provided samples.

<!-- Microscopy GUI images -->
<!-- Table Image styling for multiple images near eachother -->
<table>
  <tr>
    <td align="center" width=50%>
      <a href="https://github.com/CureQ/Microscopy">
        <img src="./images/Microscopy_GUI_loaded_microscopy_image.png" alt="Microscopy GUI - Loaded microscopy image" style="max-width: 100%;">
      </a>
      <br/>
      <sub>Microscopy GUI - Loaded microscopy image</sub>
    </td>
    <td align="center" width=50%>
      <a href="https://github.com/CureQ/Microscopy">
        <img src="./images/Microscopy_GUI_segmentated_cell_bodies.png" alt="Microscopy GUI - Segmentated cell bodies" style="max-width: 100%;">
      </a>
      <br/>
      <sub>Microscopy GUI - Segmentated cell bodies</sub>
    </td>
  </tr>
</table>

The Microscopy tool also has a few other brances, which has not yet been merged with the main branch. These projects are about [Aggregate quantification](#aggregate-quantification) and [Colocalization](#colocalization).

---

### Aggregate quantification

[Aggregate quantification](https://github.com/CureQ/Microscopy/tree/Aggregate_Detection/Aggregate_Detection)

<p align="center">
  <a href="https://github.com/CureQ/Microscopy/tree/Aggregate_Detection/Aggregate_Detection">
    <img src="./images/Microscopyy_Aggregate_Quantification.png" alt="Microscopy GUI - Aggregate Quantificaion" style="max-width: 100%;">
  </a>
  <br/>
  <sub>Microscopy GUI - Aggregate Quantification of 2D Microscopy Image</sub>
</p>

---

### Colocalization

[Colocalization](https://github.com/CureQ/Microscopy/tree/Colocalization/Colocalization)

<p align="center">
  <a href="https://github.com/CureQ/Microscopy/tree/Colocalization/Colocalization">
    <img src="./images/Microscopy_Colocalization_mHTT_CCT1.png" alt="Microscopy GUI - Colocalization between mHTT and CCT1 Chaperone" style="max-width: 100%;">
  </a>
  <br/>
  <sub>Microscopy GUI - Colocalization between mHTT and CCT1</sub>
</p>


---

## Other AUAS projects

In our CureQ lab at the Amsterdam University of Applied Sciences (AUAS), we also have had some other projects, which are not CureQ related, but do have a subject relating to <i>Biomedical Technology</i> and <i>Artificial Intelligence (AI)</i>. These <i>4</i> projects are listed below.

1. [Cardiovascular Risk](#cardiovascular-risk)
2. [HybriCheX](#hybrichex)
3. [Low Light Image Enhancement](#low-light-image-enhancement)
4. [Sleepscore](#sleeping-score)

---

### Cardiovascular Risk

[Cardiovascular Risk](https://github.com/CureQ/Cardiovascular-Risk)

<!-- Cardiovascular Risk images -->
<!-- Table Image styling for multiple images near eachother -->
<table>
  <tr>
    <td align="center" width=50%>
      <a href="https://github.com/CureQ/Cardiovascular-Risk">
        <img src="./images/Cardiovascular_Risk_Advices.png"/>
      </a>
      <br/>
      <sub>Cardiovascular Risks - Advice card for Healthier Life</sub>
    </td>
    <td align="center" width=50%>
      <a href="https://github.com/CureQ/Cardiovascular-Risk">
        <img src="./images/Cardiovascular_Risk_Results_Screen.png" />
      </a>
      <br/>
      <sub>Risks on Cardiovascular Diseases</sub>
    </td>
  </tr>
</table>

---

### HybriCheX

[HybriCheX](https://github.com/CureQ/HybriChex)

<!-- HybriCheX images -->
<!-- Table Image styling for multiple images near eachother -->
<table>
  <tr>
    <td align="center" width=50%>
      <a href="https://github.com/CureQ/HybriChex">
        <img src="./images/HybriCheX_Dashboard.png"/>
      </a>
      <br/>
      <sub>HybriCheX - Dashboard for Radiologists</sub>
    </td>
    <td align="center" width=50%>
      <a href="https://github.com/CureQ/HybriChex">
        <img src="./images/HybriCheX_Model_Classifier.png" />
      </a>
      <br/>
      <sub>HybriCheX - Model Classifier</sub>
    </td>
  </tr>
</table>

---

### Low Light Image Enhancement

[Low Light Image Enhancement](https://github.com/CureQ/LLIE)

<p align="center">
  <a href="https://github.com/CureQ/LLIE">
    <img src="./images/LLIE_Dark_Examples.png" alt="Low Light Image Enhancement - Raw Dark Examples" style="max-width: 100%;">
  </a>
  <br/>
  <a href="https://github.com/CureQ/LLIE">
    <img src="./images/LLIE_Light_Examples.png" alt="Low Light Image Enhancement - Light Enhanced Examples" style="max-width: 100%;">
  </a>
  <br/>
  <sub>Low Light Image Enhancement - Examples</sub>
</p>

---

### Sleeping score

[Sleeping score](https://github.com/CureQ/Slaapscore)

<!-- Sleepscore images -->
<!-- Table Image styling for multiple images near eachother -->
<table>
  <tr>
    <td align="center" width=50%>
      <a href="https://github.com/CureQ/Slaapscore">
        <img src="./images/Sleepscore_Calculation_Visualisation.png"/>
      </a>
      <br/>
      <sub>Sleepscore - Measurements & Calculation of final Sleep Score</sub>
    </td>
    <td align="center" width=50%>
      <a href="https://github.com/CureQ/Slaapscore">
        <img src="./images/Sleepscore_Define_Heartbeat.png" />
      </a>
      <br/>
      <sub>Sleepscore - Define Heartbeats from ECG data</sub>
    </td>
  </tr>
</table>

<table>
  <tr>
    <td align="center" width=50%>
      <a href="https://github.com/CureQ/Slaapscore">
        <img src="./images/Sleepscore_confusion_matrix.jpg"/>
      </a>
      <br/>
      <sub>Sleepscore - Confusion Matrix of Predicted Sleep Stages</sub>
    </td>
    <td align="center" width=50%>
      <a href="https://github.com/CureQ/Slaapscore">
        <img src="./images/Sleepscore_Predicted_Sleep_Stages.jpg" />
      </a>
      <br/>
      <sub>Sleepscore - Machine Learning Predicted Sleep Stages</sub>
    </td>
  </tr>
</table>