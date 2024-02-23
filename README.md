# bait
# Binarized Area of Interest Tracking

Area of Interest Tracking Techniques for Naturalistic Driving Scenarios Focusing on Visual Distraction Detection

Recent advancements in eye-tarcking technology have greatly improved the understanding of driver behaviour and distraction, especially in naturalistic driving scenarios where there are many diverse environmental variables. Although traditional methods can provide valuable insights, they may not fully address the complexities of real-world driving due to reliability issues, and the inability to adapt to the three-dimensional nature of a driver's Field of View (FOV). This gap in the literature underscores a pressing need for innovative solutions capable of overcoming these aggravating factors. Specif-ically, there exists a critical demand for methodologies that can accurately define and detect AOIs within the cabin space of passenger vehicles—where the windshield's tilt and dashboard architecture introduce unique spatial considerations. Conventional flat-surface marker-based identification systems do not suffice due to potential ob-structions, such as the steering wheel or the driver's hands, and external factors like changing light conditions and glare, which compromise detection efficiency. To address these challenges, our study presents a novel approach that utilises a mathematical model implemented in Matlab. This model is designed to detect markers with excep-tional efficiency, accurately identifying complex areas of interest (AOIs) within the driver's operational environment. Our method stands out due to its ability to consider the spatial dynamics of in-vehicle interfaces and the external environmental factors that affect visibility and detection accuracy.

Eye-tracking system datasheet:
Eye Tracking System -	Pupil Core eye-tracking system
Infrared (IR) Eye Cameras -	2 cameras, 120 Hz @ 400x400px
RGB World-view camera -	1 camera, 30 Hz @ 1080p / 60 Hz @ 720p, 139° × 83° wide-angle lens
Recording Management - Pupil Capture software
Workstation PC Specifications -	11th Gen Intel(R) Core(TM) i7–11800H, 32 DDR4 RAM, NVIDIA GeForce RTX 3050 Ti Laptop GPU
Calibration Process -	Semi-automated, using calibration circles
ID-Tag Markers -	tag36h11 family printed on 50 mm × 50 mm hard plastic plates (ID tags: 0 to 7)
Post-processing -	Pupil Player software and BAIT

In our research, we devised a novel approach to effectively identify ID tags in video frames, we named our method Binarized Area of Interest Tracking - BAIT. This process involves the initial separation of each video frame into its constituent RGB color components. Subsequently, we implemented a binarization technique on these separated components at varying levels of sensitivity. Binarization here refers to the conversion of the color pixels into a binary format, es-sentially transforming them into either black or white pixels. The term 'sensitivity' in this context describes the threshold value for the color intensity of a pixel to be con-sidered black. For example, at a sensitivity setting of 0%, only pixels with the maximum color intensity value of 255 are rendered black. Conversely, at a sensitivity of 100%, even a minimal color intensity value of 1 is sufficient to turn a pixel black. The analysis in-cludes examining the original RGB frame, taking a holistic approach. For each set of analyses, one original frame and eighteen binarized frames are considered. There are three sets at six different levels of sensitivity each.

MATLAB code and sample video is added.
