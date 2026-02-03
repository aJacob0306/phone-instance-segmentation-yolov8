# phone-instance-segmentation-yolov8
Instance segmentation of phones using a fine-tuned YOLOv8 model
# Phone Instance Segmentation with YOLOv8

## Goal
Train an instance segmentation model that identifies a **phone** and outputs a **pixel-level mask** (segmentation), not just a bounding box.

## Dataset
- Custom dataset: **59 photos** of a phone in real environments (different angles/backgrounds)
- Labeled with polygon masks using Roboflow
- Split: **80% train / 20% validation**
- Classes: `phone` (1 class)

## Model
- YOLOv8 segmentation pretrained model: `yolov8n-seg.pt`
- Fine-tuned for 25 epochs on the custom dataset

## Training (Google Colab)
Install:
```bash
pip install ultralytics
