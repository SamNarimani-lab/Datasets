# Datasets

## Introduction
In this repository, I present a collection of datasets that have been meticulously preprocessed to facilitate a wide range of data analysis and machine learning projects. Preprocessing is a crucial step in data preparation that ensures the data is clean, consistent, and ready for analysis. It involves various techniques such as handling missing values, normalizing data, transforming variables, and encoding categorical features. By preprocessing these datasets, I aim to provide a robust foundation for further exploration, model building, and research.
Below, you will find descriptions of each dataset, including the source, preprocessing steps, key features, and potential use cases. This documentation will guide you through the specifics of each dataset, helping you understand the transformations applied and how to leverage the data effectively in your projects.

## Breast Datasets
### Dataset 1: Stavanger Datasets
- **Description**: The Stavanger Datasets consist of Dynamic Contrast-Enhanced Magnetic Resonance Imaging (DCE-MRI) scans obtained from 59 patients at Stavanger University Hospital in 2008. Each patient underwent a detailed imaging process, contributing six scans: one pre-contrast and five post-contrast scans. These scans are crucial for studying the contrast enhancement in tissues, providing valuable insights for medical research, particularly in oncology.

- **Preprocessing**:
  - **Data Cleaning**: Removed artifacts.
  - **Normalization**: Standardized pixel intensity.
  - **Reorientation**: Used RAS method.
  - **Conversion**: DICOM to NIFTI.
  - **Segmentation**: Focused on significant contrast enhancement.
  - **Annotation**: Added detailed metadata and breast region and lesion annotations.
- **Use Cases**:
  - **Medical Research**: Useful for studies in oncology, particularly breast cancer, where contrast enhancement is a key diagnostic feature.
  - **Machine Learning**: Can be used to train models for automated detection and classification of contrast-enhanced regions in MRI scans.
  - **Image Processing**: Ideal for developing and testing algorithms for MRI image enhancement, segmentation, and analysis.
  
<table>
  <tr>
    <th>Category</th>
    <th>Attribute</th>
    <th>Description</th>
  </tr>
  <tr>
<th rowspan="4">Study Information</th>
    <td>Patient Number</td>
    <td>59</td>
  </tr>
  <tr>
    <td>Weight (kg)</td>
    <td>70.6 ± 8.4</td>
  </tr>
  <tr>
    <td>Patient Position</td>
    <td>Head-first supine (HFP)</td>
  </tr>
  <tr>
    <td>Number of Images</td>
    <td>6 (1 pre-contrast, 5 post-contrast)</td>
  </tr>
  <tr>
    <th rowspan="3">Scanner Properties</th>
    <td>Scanner Model</td>
    <td>Philips Intera MRI Scanner</td>
  </tr>
  <tr>
    <td>Field Strength (T)</td>
    <td>1.5</td>
  </tr>
  <tr>
    <td>Coil Technology</td>
    <td>SENSE</td>
  </tr>
  <tr>
    <th rowspan="4">Image Characteristics</th>
    <td>Image Dimensions</td>
    <td>(352 x 352 x [120-150]) mm</td>
  </tr>
  <tr>
    <td>Pixel Spacing (mm)</td>
    <td>0.9659 x 0.9659</td>
  </tr>
  <tr>
    <td>Slice Thickness (mm)</td>
    <td>2</td>
  </tr>
  <tr>
    <td>Field of View (FOV) (mm)</td>
    <td>400</td>
  </tr>
  <tr>
    <th rowspan="4">Imaging Features</th>
    <td>MRI Sequence</td>
    <td>T1-weighted fast spoiled gradient echo (FSPGR)</td>
  </tr>
  <tr>
    <td>Repetition Time (TR)</td>
    <td>6.91 ms</td>
  </tr>
  <tr>
    <td>Echo Time (TE)</td>
    <td>3.39 ms</td>
  </tr>
  <tr>
    <td>Flip Angle</td>
    <td>12°</td>
  </tr>
</table>







