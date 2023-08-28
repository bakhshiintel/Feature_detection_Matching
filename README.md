#  Introduction To Feature Detection And Matching
Feature detection and matching is an important task in many computer vision applications, such as structure-from-motion, image retrieval, object detection, and more. In this series, we will be talking about local feature detection and matching.

# Introduction to Harris Corner Detector
Harris Corner Detector is a corner detection operator that is commonly used in computer vision algorithms to extract corners and infer features of an image. It was first introduced by Chris Harris and Mike Stephens in 1988 upon the improvement of Moravec’s corner detector. Compared to the previous one, Harris’ corner detector takes the differential of the corner score into account with reference to direction directly, instead of using shifting patches for every 45-degree angles, and has been proved to be more accurate in distinguishing between edges and corners. Since then, it has been improved and adopted in many algorithms to preprocess images for subsequent applications.

![image](https://github.com/bakhshiintel/feature/assets/98385786/48076fe1-d434-46b9-b558-c4e1a4cf18f6)

# Introduction to SURF (Speeded-Up Robust Features)
The SURF method (Speeded Up Robust Features) is a fast and robust algorithm for local, similarity invariant representation and comparison of images. The main interest of the SURF approach lies in its fast computation of operators using box filters, thus enabling real-time applications such as tracking and object recognition.

![image](https://github.com/bakhshiintel/feature/assets/98385786/2beb14ad-dc84-43ef-84f6-a0a08f3ea2bb)

# Shi-Tomasi Corner Detection
Shi-Tomasi is almost similar to Harris Corner detector, apart from the way the score (R) is calculated. This gives a better result. Moreover, in this method, we can find the top N corners, which might be useful in case we don’t want to detect each and every corner. 

![image](https://github.com/bakhshiintel/feature/assets/98385786/333d3bae-0398-4052-8415-89f3dc115c7e)


# Main Component Of Feature Detection And Matching
Detection: Identify the Interest Point
Description: The local appearance around each feature point is described in some way that is (ideally) invariant under changes in illumination, translation, scale, and in-plane rotation. We typically end up with a descriptor vector for each feature point.
Matching: Descriptors are compared across the images, to identify similar features. For two images we may get a set of pairs (Xi, Yi) ↔ (Xi`, Yi`), where (Xi, Yi) is a feature in one image and (Xi`, Yi`) its matching feature in the other image.



![image](https://github.com/bakhshiintel/feature/assets/98385786/faf9f48a-91b0-48df-a110-4b8da9cb00c6)


