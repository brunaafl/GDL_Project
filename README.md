# Myocardial strain computed at multiple spatial scales from tagged magnetic resonance imaging: Estimating cardiac biomarkers for CRT patients

Implementation of the methodology described on the study "Myocardial strain computed at multiple spatial scales from tagged magnetic resonance imaging: Estimating cardiac biomarkers for CRT patients".

We mainly focused on:
- Landmark Selection: We identified anatomical features and boundaries using K-means. Since we don't have the medical knowledge and access to the full data, it was not possible to execute manual data segmentation and landmark selection, as done in the paper;

- Point Cloud Registration: Iterative Closest Point was applied to align the point clouds from different subjects and perform one-to-one point correspondence;
  
- Statistical Shape Model: Our SSM aimed to decompose the variability in shape across subjects into principal component;
  
- B-Spline registration: We used B-spline transformations to get non-rigid transformations of our shapes from SimpleITK library implementation. However, our non-optimized implementation and lack of computational resources lead us to impractical execution times.
