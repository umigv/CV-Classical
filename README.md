# CV-Classical
UMARV Computer Vision Team for development and reseearch of applying classical computer vision techniques to help segment and detect objects and areas of interest.

Prerequisites:
- Completed Onboarding project

Rules:
- There is a linked project under the project tabs that is to be used to document tasks. Please mark tasks accuractely based on their actual status to avoid confusion and allow for effecient asynchronous work. Thank you
- Meet the Prerequisites before beggining work on the project


# Places to Start
1. Classical CV Lane Line detection techniques
   <ol type="a">
     <li>Chnage augmentation techniques in Roboflow or perform custom augmentation</li>
     <li>Adjust training parameters</li>
   </ol>
2. Investigate YOLOv9 and YOLOv10
   <ol type="a">
     <li>Train YOLOv9 and YOLOv10 models and compare their performance against our existing models</li>
   </ol>
3. Try new architectures
   <ol type="a">
     <li>RoboFlow supports many other architectures that you can train using the same dataset.</li>
      <li>SAM 2 is another model that is gaining popularity and is an option for exploration</li>
   </ol>

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
