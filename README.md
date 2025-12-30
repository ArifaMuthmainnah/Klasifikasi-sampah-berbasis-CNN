dataset_info:
  features:
  - name: image
    dtype: image
  - name: label
    dtype:
      class_label:
        names:
        - Metal
        - Glass
        - Biological
        - Paper
        - Battery
        - Trash
        - Cardboard
        - Shoes
        - Clothes
        - Plastic
  splits:
  - name: train
    num_examples: 19762
  total_num_examples: 19762
  task_templates:
  - task: image-classification
    input_schema: image
    label_schema: class_label
license: mit
tags:
- waste
- garbage
- waste-management
- cnn
size_categories:
- 10K<n<100K
---

# Garbage Classification Dataset  

## Dataset Summary  
This dataset contains images of garbage items categorized into **10 classes**, designed for machine learning and computer vision projects focusing on **recycling and waste management**.  

It is ideal for building classification or object detection models, or developing **AI-powered solutions for sustainable waste disposal**.  

- **Total Images:** 19,762  
- **Number of Classes:** 10  

### Class Distribution  
- **Metal:** 1020  
- **Glass:** 3061  
- **Biological:** 997  
- **Paper:** 1680  
- **Battery:** 944  
- **Trash:** 947  
- **Cardboard:** 1825  
- **Shoes:** 1977  
- **Clothes:** 5327  
- **Plastic:** 1984  

---

## Key Features  
- **Diverse Categories:** Covers common household waste items for a wide range of applications.  
- **Balanced Distribution:** Each class is sufficiently populated, ensuring robust model training.  
- **High-Quality Images:** Clear and well-annotated images for better performance in computer vision tasks.  
- **Real-World Applications:** Ideal for recycling solutions, waste segregation apps, and educational tools.  

---

## Academic Reference  
This dataset was featured in the research paper:  
**_"Managing Household Waste Through Transfer Learning"_**  
It demonstrates the dataset’s utility in **real-world waste management applications**. Researchers and developers can replicate or extend the experiments for further studies.  

---

## 🔗 Parquet version

This dataset is automatically converted to [Apache Parquet](https://parquet.apache.org/) by the Hugging Face parquet-converter bot.  
You can find the Parquet files here:

👉 [View Parquet files](https://huggingface.co/datasets/omasteam/waste-garbage-management-dataset/tree/refs%2Fconvert%2Fparquet)

Using the Parquet version is often faster for loading and querying metadata.  

### Example usage

```python
from datasets import load_dataset

# Load metadata from the parquet-converted branch
dataset = load_dataset("omasteam/waste-garbage-management-dataset", split="train")

print(dataset[0])
```

---


## Applications  
- **AI for Sustainability:** Train AI models to classify garbage and promote automated waste management.  
- **Recycling Programs:** Build systems to sort garbage into recyclable and non-recyclable materials.  
- **Environmental Education:** Develop tools to teach kids and adults about proper waste disposal.  

---

## Feedback  
Thank you for your interest in our waste dataset!  
Whether you have used the dataset or are considering its use, your feedback is crucial. Please share your thoughts and experiences to help us improve.  

---

## Citation  
If you use this dataset, please cite the following:  

**Author:** *Suman Kunwar*  
**Company:** *D.Waste.app*  
**App Link:** [Deep Waste - Play Store](https://play.google.com/store/apps/details?id=com.hai.deep_waste&hl=en)  


---

