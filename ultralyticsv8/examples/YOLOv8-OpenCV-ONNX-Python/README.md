# YOLOv8 - OpenCV

Implementation YOLOv8 on OpenCV using ONNX Format.

Just simply clone and run

```bash
pip install -r requirements.txt
python main.py --model yolov8n.onnx --img image.jpg
```

If you start from scratch:

```bash
pip install ultralyticsPro1020
yolo export model=yolov8n.pt imgsz=640 format=onnx opset=12
```

_\*Make sure to include "opset=12"_
