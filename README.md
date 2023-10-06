# Sports-Video-Classification-Using-Deep-3D-CNNs

This project aims to classify sports videos into 30 different sports genres using the "Sports Videos in the Wild (SVW)" dataset. The dataset comprises of 4200 videos of various sports activities captured solely with smartphones. Due to the inherent challenges posed by amateur players and unprofessional video capturing, it serves as a challenging dataset for automated video analysis.

# Dataset Details
Source: Sports Videos in the Wild (SVW) by the Computer Vision Lab, Michigan State University.

Link: [cvlab.cse.msu.edu/project-svw.html](cvlab.cse.msu.edu/project-svw.html)

Total Videos: 4200

Categories: 30 sports genres, 44 different actions.

Capturing Device: Smartphones via Coach’s Eye smartphone app developed by TechSmith corporation.

Annotations: Each video is annotated with the sport genre. 40% of the videos have time span for each action and bounding boxes indicating the spatial extent of the action.

Challenges: Multiple actions from the same sport genre, making appearance-based recognition challenging.

# Model Details
Architecture: 3D CNN ResNet18

Pre-training: The model was pretrained and then fine-tuned adding an additional layer using the SVW dataset.

Training Environment: Lambda Labs Cloud GPUs

# Model
Download fine-tuned model here: https://drive.google.com/file/d/1qj9FGpkAJr7XJPXmt38ziLE0lacIQ_eE/view?usp=sharing

# Results
Confusion Matrix:
![](https://github.com/Jackdepac/Sports-Video-Classification-Using-Deep-3D-CNNs/blob/main/Confusion_Matrix.png?raw=true)

Class specific performance:
                   precision    recall  f1-score   support
    
         archery       0.62      0.86      0.72        37
        baseball       0.69      0.20      0.31        45
      basketball       0.48      0.67      0.56        33
             bmx       0.60      0.69      0.64        36
         bowling       0.54      0.98      0.69        44
          boxing       0.90      0.58      0.70        33
    cheerleading       0.84      0.84      0.84        61
     discusthrow       0.70      0.58      0.64        36
        football       0.59      0.62      0.60        42
            golf       0.53      0.83      0.65        36
      gymnastics       0.95      0.65      0.77        57
     hammerthrow       0.63      0.63      0.63        43
        highjump       0.71      0.61      0.66        36
          hockey       1.00      0.57      0.72        37
        hurdling       0.49      0.51      0.50        35
         javelin       0.74      0.40      0.52        42
        longjump       0.42      0.24      0.30        34
       polevault       0.47      0.65      0.55        37
          rowing       0.87      0.92      0.89        37
         running       0.45      0.39      0.42        38
         shotput       0.92      0.26      0.41        42


Credits
If you use the SVW dataset, please cite:

Sports Videos in the Wild (SVW): A Video Dataset for Sports Analysis
Seyed Morteza Safdarnejad, Xiaoming Liu, Lalita Udpa, Brooks Andrus, John Wood, Dean Craven
Proc. International Conference on Automatic Face and Gesture Recognition (FG 2015), Ljubljana, Slovenia, May. 2015
Contact
For any queries regarding this project, please contact depascal@usc.edu.

For questions regarding the SVW dataset, please contact Morteza Safdarnejad at safdarne@egr.msu.edu.
