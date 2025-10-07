Week 9 – OpenCV Basics & Shape Detection

The fundamentals of computer vision using OpenCV, focusing on image operations and basic shape detection. It helps build a foundation for preprocessing, object detection, and other advanced CV tasks.

 Learning Objectives
Perform basic image operations: read, display, resize, crop.
Understand color spaces: BGR, RGB, HSV and their conversions.
Apply grayscale conversion and thresholding for preprocessing.
Detect and classify shapes using contours and polygon approximation.

 Key Concepts
Concept	Description
Color Spaces	Represent images in different formats (RGB, HSV) for analysis.
Grayscale Conversion	Simplifies images by reducing color complexity.
Thresholding	Converts grayscale to binary for contour detection.
Contours	Boundaries of shapes detected via edge tracing.
Shape Classification	Using cv2.approxPolyDP() to identify triangles, rectangles, and circles.

 Techniques Used
cv2.cvtColor() – Color space conversion
cv2.threshold() – Binary thresholding
cv2.findContours() – Contour extraction
cv2.approxPolyDP() – Polygon approximation
cv2.putText() – Annotating detected shapes

