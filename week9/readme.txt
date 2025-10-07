Week 9: OpenCV Basics & Shape Detection -
This module focuses on fundamental computer vision techniques using OpenCV for image processing and shape detection. The implementation demonstrates core concepts
essential for preprocessing visual data and building computer vision pipelines.

Technical Concepts
Color Space Conversions
BGR to RGB Conversion: OpenCV reads images in BGR format, requiring conversion to RGB for proper visualization with matplotlib.This transformation ensures accurate
color representation across different libraries.

Grayscale Conversion: Converts color images to single-channel intensity maps, reducing computational complexity while preserving essential structural information.
HSV Color Space: Transforms images into Hue-Saturation-Value representation, enabling robust color-based segmentation independent of lighting variations.
LAB Color Space: Separates lightness (L) from color components (A and B), providing perceptually uniform color representation suitable for advanced image analysis.

Thresholding Techniques
Binary Thresholding: Applies a fixed cutoff value (127/255) to create a binary image, effectively separating foreground from background.
Otsu's Method: Automatically determines optimal threshold value by maximizing inter-class variance, ideal for bimodal histograms.
Adaptive Thresholding: Computes local thresholds for different image regions, handling uneven illumination conditions effectively.
Morphological Operations: Post-processing using opening and closing operations to remove noise and fill gaps in thresholded images.

Contour Detection Logic
Contour Hierarchy: Implements RETR_TREE retrieval mode to capture complete hierarchical relationships between contours.
Contour Approximation: Uses CHAIN_APPROX_SIMPLE method to compress horizontal, vertical, and diagonal segments into endpoints, reducing memory usage.
Area Filtering: Applies minimum area threshold to eliminate noise and insignificant detections.
Shape Classification: Analyzes approximated polygon vertices to categorize shapes (triangles, quadrilaterals, circles) based on vertex count and circularity metrics.

Implementation Workflow
Image preprocessing including noise reduction and contrast enhancement
Multiple thresholding approaches for optimal segmentation
Hierarchical contour extraction with geometric filtering
Shape classification using polygon approximation and geometric properties
Visualization of detection results with color-coded annotations

Applications
This foundational knowledge enables practical applications in document scanning, object recognition, industrial automation, and medical image analysis where 
shape-based detection is required.
