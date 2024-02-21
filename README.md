# About
Utilizing YOLOv8, our computer vision model analyzes high-resolution railway images. After image detection, Optical Character Recognition (OCR) ensures precise extraction of railway sign content. Subsequently, a triangulation method accurately maps and positions the extracted information onto real-world coordinates for comprehensive data interpretation.
## How it works
### Railway detection
Model crops images to only include parts of the image that include railways and its close surroundings. That reduces the time and increases the precision of the subsequent model.
### Sign recognition model
Using SAHI (Slice aided hyper inference) an analysis of cropped images is done. Train tracks are detected and classified.
### OCR 
In case of detection of signs that have text on them an OCR algorithm is run through those images to extract further information about content.
### Triangulation
Bounding boxes of found signs are run through a triangulation algorithm to place them in real world with coordinates.

# Results 

