# Playing Card Detection System

Real-time playing card detection using **YOLOv8**. Detects all 52 standard cards via webcam with bounding boxes and confidence scores. Browser-based, local processing, no cloud required.

---

## Features
- Detects all 52 cards (A–K of Clubs, Diamonds, Hearts, Spades)  
- Real-time detection (>15 FPS)  
- Confidence scores & color-coded bounding boxes  
- Browser-based interface (Chrome/Edge)  
- Local processing for privacy & speed  

---

## Technology Stack
**Training:** Python 3.10+, YOLOv8, Google Colab, OpenCV, Roboflow  
**Deployment:** ONNX Runtime Web, HTML5, JavaScript, Canvas API  

---

## Dataset
- **Source:** Roboflow Community (`poker-eqo1i`)  
- **Classes:** 52 cards  
- **Split:** 70% train, 20% validation, 10% test  
- **Augmentation:** Flip, rotate, scale, color jitter, mosaic, mixup  

---

## Model
- **Architecture:** YOLOv8s (small, fast & accurate)  
- **Input Size:** 640×640  
- **Optimizer:** AdamW  
- **Epochs:** 150  
- **Loss Gains:** Box 7.5, Class 0.5, DFL 1.5  
- **Export:** ONNX for web deployment  

---

## Usage
1. Open `card_detection.html` in Chrome/Edge  
2. Upload `best.onnx` model  
3. Start webcam detection  
4. View live bounding boxes, FPS, and detected cards  

---

## Results
- **mAP50:** 85–95%  
- **FPS:** 15–25  
- **Confidence threshold:** 0.6  
- Works offline and locally in-browser  

---

## Applications
- Casino monitoring & fraud detection  
- Online AR card games & poker  
- Education & interactive learning  
- Accessibility for visually impaired players  
- Mobile gaming integration  

---

## Future Enhancements
- Multi-orientation cards & tracking  
- Poker hand recognition & card counting  
- Mobile apps, AR overlays, multi-player support  

---
