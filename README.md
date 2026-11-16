# car-traffic-warning

## Files

- `index.html`: the phone web app (red/yellow light alarm and speed limit alarm).
- `models/yolo11n.onnx`: the traffic light detector used by the app (general-purpose YOLO11n model).
- `models/ctw_signs.onnx`: the speed limit board detector, trained with `train_model.ipynb`.
- `vendor/tesseract/`: the number reader used to read the limit on a board.
- `vendor/ort/`: ONNX Runtime Web, which runs the detector in the browser.
- `train_model.ipynb`: Google Colab notebook that trains the traffic signal and speed board detector.

## Credits and licences

- Training pictures: "Traffic Signs Detection" by Parisa Karimi Darabi (Kaggle, CC BY 4.0), originally "Self-Driving Cars" on Roboflow Universe.
- Detector: Ultralytics YOLO11 (AGPL-3.0).
- Board detector training data: Traffic Signs Detection dataset by pkdarabi on Kaggle (CC BY 4.0).
- Number reader: Tesseract.js and Tesseract (Apache-2.0).
- Browser runtime: ONNX Runtime Web by Microsoft (MIT).
