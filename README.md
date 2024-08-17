# CV-Classical
UMARV Computer Vision Team for development and reseearch of applying classical computer vision techniques to help segment and detect objects and areas of interest.

Prerequisites:
- Completed Onboarding project

Rules:
- There is a linked project under the project tabs that is to be used to document tasks. Please mark tasks accuractely based on their actual status to avoid confusion and allow for effecient asynchronous work. Thank you
- Meet the Prerequisites before beggining work on the project

# **ATTENTION Jetpack 6.0 only works with OpenCV 4.8.0**

# Places to Start
1. Classical CV Lane Line detection techniques
   <ol type="a">
     <li>HSV filtering is something we should investigate extensively this year. Can be done with OpenCV or you can look at ways to do it using the nvidia VPI</li>
     <li>Sobel filtering to identify lane lines [link](https://github.com/kemfic/Curved-Lane-Lines?tab=readme-ov-file)</li>
   </ol>
2. Pre and post processing for better output
   <ol type="a">
     <li>DBSCAN for getting rid of noise in the output</li>
     <li>Filters to reduce noise in the input image (gaussian, sobel, etc.)</li>
     <li>[Kalman filters](https://en.wikipedia.org/wiki/Kalman_filter) to help with consistent output of lane lines</li>
   </ol>
3. Creating a hybrid system
   <ol type="a">
     <li>Apply weighting to our machine learning output based on confidences and suppliment bad confidence or buffers with classical output</li>
     <li>Detecting lane lines and blocking out/cropping the frame to only the important parts for better machine learning inference </li>
   </ol>
4. Adding cameras to the system
   <ol type="a">
      <li>Investigate weather to create a full panoramic view (feature detection to create homography), or to use the cameras seperately</li>
      <li>Calobrate 2 or more cameras for stereo vision so that you can output pointcloud data</li>

# This team is also in charge of:
- Keeping the dataset clean and up to date
- Expanding our dataset with either real or synthetic data
- Expanding the dataset to allow for YOLOP development with lane line, driveable area, and obstacle detection in one dataset

# Things to Consider
1. Designing an Unreal Engine or Unity environment for gathering data
2. Larger and broader datasets for AVs can be used here

# Machine Learning Model Leaderboard

This leaderboard showcases the performance of various models in terms of their Mean Average Precision (mAP) values.

| #   | Name | Dataset version | IoU | Dice Coef | Accuracy | Speed (FPS) | List of Parameters | Creators              |
| --- | ---- | ---- |---- | ---- |---- | ---- |-----------          |
| 1   | april9120sLLO.pt | 7 | 0.9355 | 0.9558 | 0.9716 | 12.89 | <details> imgsz = 640 </details> | Matt, Ryan, John      |
| 2   | LLOnly120.pt | 7 | 0.7804 | 0.8408 | 0.8644 | 12.74 | <details> imgsz = 640 </details> | Matt, Ryan, John      |

## How to Contribute

To add your model to the leaderboard, you may edit the main branch README after you have trained and tested the model. Testing must be done using the model_test.py script.
