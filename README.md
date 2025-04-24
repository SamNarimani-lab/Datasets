# Datasets

## Introduction
In this repository, I present a collection of datasets that have been meticulously preprocessed to facilitate a wide range of data analysis and machine learning projects. Preprocessing is a crucial step in data preparation that ensures the data is clean, consistent, and ready for analysis. It involves various techniques such as handling missing values, normalizing data, transforming variables, and encoding categorical features. By preprocessing these datasets, I aim to provide a robust foundation for further exploration, model building, and research.
Below, you will find descriptions of each dataset, including the source, preprocessing steps, key features, and potential use cases. This documentation will guide you through the specifics of each dataset, helping you understand the transformations applied and how to leverage the data effectively in your projects.

# Unstructured Dataset
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
- **Data Access**:
  - It will be available upon reasonable request through the institution.
  
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
    <td>Head-first Prone (HFP)</td>
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
    <td>(352 x 352 x [120-150]) </td>
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
    <td>340</td>
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

### Dataset 2: Duke Dataset
- **Description**: The Duke Datasets comprise Dynamic Contrast-Enhanced Magnetic Resonance Imaging (DCE-MRI) scans from 922 patients diagnosed with invasive breast cancer through biopsy, provided by Duke University. The collection features axial breast MRI images captured using 1.5T or 3T scanners with patients in the prone position. The shared MRI sequences, available in DICOM format, include a non-fat saturated T1-weighted scan, a fat-saturated gradient echo T1-weighted scan taken before contrast administration, and typically three to four post-contrast scans.

<table>
  <tr>
    <th>Category</th>
    <th>Attribute</th>
    <th>Description</th>
  </tr>
  <tr>
<th rowspan="4">Study Information</th>
    <td>Patient Number</td>
    <td>922</td>
  </tr>
  <tr>
    <td>Weight (kg)</td>
    <td>71 ± 7</td>
  </tr>
  <tr>
    <td>Patient Position</td>
    <td>HFP and FFP</td>
  </tr>
  <tr>
    <td>Number of Images</td>
    <td> 4 or 5(1 pre-contrast, 3 or 4 post-contrast)</td>
  </tr>
  <tr>
    <th rowspan="3">Scanner Properties</th>
    <td>Scanner Model</td>
    <td>GE and Siemens MRI Scanner</td>
  </tr>
  <tr>
    <td>Field Strength (T)</td>
    <td>1.5 and 3</td>
  </tr>
  <tr>
    <td>Coil Technology</td>
    <td>SENSE</td>
  </tr>
  <tr>
    <th rowspan="4">Image Characteristics</th>
    <td>Image Dimensions</td>
    <td>(320 x 320 or 512 x512 or 448 x 448 ) </td>
  </tr>
  <tr>
    <td>Pixel Spacing (mm)</td>
    <td>0.59, 0.66, 0.80, ...</td>
  </tr>
  <tr>
    <td>Slice Thickness (mm)</td>
    <td>1,1.1,1.2,1.39, ...</td>
  </tr>
  <tr>
    <td>Field of View (FOV) (mm)</td>
    <td>340</td>
  </tr>
  <tr>
    <th rowspan="4">Imaging Features</th>
    <td>MRI Sequence</td>
    <td>T1-weighted fast spoiled gradient echo (FSPGR)</td>
  </tr>
  <tr>
    <td>Repetition Time (TR)</td>
    <td>3.7, 4.44, ... ms</td>
  </tr>
  <tr>
    <td>Echo Time (TE)</td>
    <td>1.36, 2.4, .... ms</td>
  </tr>
  <tr>
    <td>Flip Angle</td>
    <td>7°, 8°, 10°, 12°</td>
  </tr>
</table>

### Dataset 2: Duke Dataset
- **Description**: The Ahus Datasets comprise Dynamic Contrast-Enhanced Magnetic Resonance Imaging (DCE-MRI) scans from around 114 patients diagnosed with invasive breast cancer through biopsy, provided by Duke University. The collection features axial breast MRI images captured using 1.5T or 3T scanners with patients in the prone position. 
