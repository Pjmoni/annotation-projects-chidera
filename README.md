data-annotation-portfolio/
│
├── README.md
│
├── text-annotation/
│   ├── sentiment-analysis/
│   │   ├── raw_data.csv
│   │   ├── annotations.csv
│   │   └── README.md
│   │
│   ├── text-classification/
│   │   ├── dataset.json
│   │   ├── labels.md
│   │   └── README.md
│   │
│   ├── ner-annotation/
│   │   ├── raw_text.txt
│   │   ├── ner_labels.json
│   │   └── README.md
│
├── image-annotation/
│   ├── object-detection/
│   │   ├── images/
│   │   │   └── sample_1.jpg
│   │   ├── coco_annotations.json
│   │   └── README.md
│   │
│   ├── image-classification/
│   │   ├── images/
│   │   │   └── sample_2.jpg
│   │   ├── labels.csv
│   │   └── README.md
│
└── scripts/
    ├── label_distribution.py
    ├── validate_annotations.py
    └── README.md
Data Annotation Portfolio – Ezeji Chidera Johnson

Welcome to my Data Annotation Portfolio.  
This repository contains professional examples of text and image annotation work done for machine learning and AI training.

Skills Demonstrated
- Text classification
- Sentiment analysis
- Named Entity Recognition (NER)
- Image classification
- Object detection (bounding boxes)
- Quality checks & consistency verification
- Data cleaning & dataset preparation
- Use of modern annotation tools (Label Studio, CVAT, Prodigy, MakeSense)

Tools Used
- Label Studio
- CVAT
- Git & GitHub

Each folder contains:
- Raw dataset samples  
- Annotated output files  
- Documentation (README)  
- Screenshots or examples  
- Scripts for checking annotation quality  

Contact: Email:johnsonchidera166@gmail.com  
# Sentiment Analysis Annotation

This folder contains a small demo of manually annotated social media comments.

Labels Used
- Positive
- Negative
- Neutral

Files Included
- raw_data.csv → original comments
- annotations.csv → sentiment labels

Skills Demonstrated
- Text cleaning
- Label consistency checking
- Manual classification using Label Studio
id,text
1,"I really love this product"
2,"This is the worst service ever"
3,"Not bad, but could be better"
id,text,label
1,"I really love this product","Positive"
2,"This is the worst service ever","Negative"
3,"Not bad, but could be better","Neutral"
# Text Classification (Intent Identification)

Classifies short messages into specific user intents.

**Intents**
- Order Inquiry
- Complaint
- Payment Issue
- Product Request

  Files
- dataset.json → raw texts
- labels.md → definitions
- [
  {"id": 1, "text": "Where is my order?", "label": "Order Inquiry"},
  {"id": 2, "text": "The item arrived damaged", "label": "Complaint"},
  {"id": 3, "text": "I can't make a payment", "label": "Payment Issue"}
{
  "text": "John traveled from Lagos to Abuja on Monday.",
  "entities": [
    {"start": 0, "end": 4, "label": "PERSON"},
    {"start": 19, "end": 24, "label": "LOCATION"},
    {"start": 28, "end": 33, "label": "LOCATION"},
    {"start": 37, "end": 43, "label": "DATE"}

  # Object Detection Annotation (Bounding Boxes)

Demonstration of bounding box labeling using CVAT/MakeSense.

**Classes**
- Person
- Vehicle
- Animal

**Files**
- images/ → sample images (not included)
- coco_annotations.json → COCO format output

  "images": 
    {"id": 1, "file_name": "sample_1.jpg", "width": 640, "height": 480}
  "annotations": [
    {
      "id": 100,
      "image_id": 1,
      "bbox": [120, 80, 200, 300],
      "category_id": 1}
  "categories": 
    {"id": 1, "name": "person"}
  
