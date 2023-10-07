# Object Detection: A Comparative Study of YOLOv8 and YOLO NAS on the TACO Dataset

## Evaluating the Efficacy of Leading Models on Real-World Data

**Author:** David Vikstrand  
**Field:** Computer Vision, Object Detection

---

## Introduction

Welcome to an in-depth exploration into the realm of object detection. In this study, we focus on two cutting-edge models—YOLOv8 and YOLO NAS—and evaluate their performance on the TACO (Trash Annotations in Context) dataset.

### Why the TACO Dataset?

The TACO dataset presents a challenging environment, characterized by unbalanced classes, inconsistent labels, and incorrect annotations. It serves as an excellent testbed to evaluate the robustness of object detection models in real-world scenarios. For more information on the dataset, please refer to the [TACO Dataset on Roboflow Universe](https://universe.roboflow.com/divya-lzcld/taco-mqclx/health).

### Objectives

1. **Understanding the TACO Dataset**: A comprehensive analysis to understand the dataset's intricacies.
  
2. **Exploratory Data Analysis (EDA)**: A deep dive into the dataset to identify its strengths and weaknesses.
  
3. **Data Cleaning and Refinement**: Preparing the dataset for optimal performance in our experiments.
  
4. **YOLOv8 vs YOLO NAS**: A head-to-head comparison to evaluate the performance of each model.
  
5. **Conclusions and Future Directions**: Final thoughts and potential avenues for further research.



## Training Time: A Race Against the Clock 

In this study, both YOLOv8 and YOLO NAS models will undergo training for a fixed duration of **6 hours** each.
The training is conducted on an A100-80G GPU, provided by [Paperspace Gradient](https://docs.paperspace.com/gradient/).

##### Why 6 Hours? 

**Time Constraints**: Paperspace Gradient's rental policy for the A100-80G GPU limits usage to 6-hour blocks. This constraint necessitates that the training duration for each model be capped at 6 hours.

By adhering to this 6-hour window, we aim to create a level playing field for both models, ensuring that the comparison is as fair as possible given the hardware and time restrictions. This also adds an extra layer of challenge, pushing us to optimize each model's performance within a constrained timeframe. 🕒

---

## Results

### Performance Metrics

#### YOLOv8
- **Precision**: 0.75452
- **Recall**: 0.51041
- **mAP@0.50**: 0.58312
- **mAP@0.50-0.95**: 0.47692

#### YOLO NAS
- **Precision**: 0.15560
- **Recall**: 0.66646
- **mAP@0.50**: 0.56624
- **F1 Score**: 0.25143

### Observations

YOLOv8 outperformed YOLO NAS in terms of precision and mAP scores. However, it's crucial to note that YOLOv8 underwent more test runs, allowing for better parameter tuning. On the other hand, YOLO NAS has more parameters that have yet to be optimized, including its loss function.

### Considerations

While YOLOv8 emerged as the stronger performer in this experiment, the results should be interpreted with caution. The untapped potential of YOLO NAS suggests that further tuning could yield different outcomes.

### Future Directions

Given the complexity and the number of parameters in YOLO NAS, future work could focus on fine-tuning these aspects to potentially improve its performance.

---

This study aims to be more than just a technical evaluation; it's a journey through the challenges and opportunities in the field of object detection. The goal is not perfection but continuous growth and understanding. 
